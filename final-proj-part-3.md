# Final Project Part 3: Data Processing, Setbacks, and a Website
[Back to Part 1](kelp-proj-HNeblina.md)

[Back to Part 2](final-part-2.md)

[Back to Portfolio](README.md)

[My Kelp Website](https://carnegiemellon.shorthandstories.com/070951e8-c3d6-49d9-8166-4a097fa5b8f1/index.html)

## Big Data, Big Hassle
The most interesting data I used for this project was a collection of 30 by 30 meter raster cells tracking kelp forest biomass for the entire US West Coast, as well as a big chunk of the Pacific Ocean. When I first found these data, I was relieved--it was just what I needed. 

However, it was not easy to handle. To start, the file size was so large that it took over an hour just to download the data, though it was no surprise that such an expansive swath of satellite imagery would be cumbersomely large. What was more of an obstacle was the file type: NetCDF. I had never seen it before, let alone used it in a project. After doing some research, I learned two things. First, NetCDF files for this type of imagery usually held time-series raster data, exactly what I hoped for. Second, they were a hassle to use in general and specifically in ArcGIS Pro, where I intended to make a large portion of my visualizations.

I tried to use the raster data as intended. I imported it into my project, and I tried to make a mosaic data set that contained information on each year--over and over again. One of the tools in ArcGIS ran for seven and a half hours. It failed. After what must have been at least a dozen hours of failed geoprocessing, I took the advice of my professor, Dr. Goranson, and tried to convert the NetCDF rasters to points. That failed, too. However, I did manage to extract the information as a table (on the second or third try), and I knew I could run the XY Table to Point tool to make a point layer the way I wanted to. 

I wrote some Python code in a notebook within my project. One cell selected all the records for each year and created a new table for each. That took about 2 and a half hours. The next cell took each one of those new tables and ran the XY Table to Point tool so I would have point-information for each year's kelp forest. That took about 7 hours. But, after one or two dozen hours of (mostly failed) data processing, I had the information I needed to make my data visualizations.

It was at this point that I spilled water all over my laptop.

I lost all my progress and had to start over--not only on this, but on every other project I had been working on up to that point. This meant that I had to scale down my ambitions for my project, but I was confident I would still be able to use the data I wanted, just not with as much depth. I rewrote my python code, processed the NetCDF data again, and gathered the rest of my data from other sources. At that point, I could implement some of the changes that I wanted to make since Part 2, albeit with significantly less sleep.


## Finishing the Project
One of the best things I got out of my interviews was insight as to who my target audience would be. Before the interviews, I was unsure of who exactly I would want to see my website. Policymakers as an audience didn't make much sense. Besides funneling money into research, they couldn't really do anything about it. After all, how would they help sick starfish at the bottom of the sea? An academic audience could have worked, but after losing all my progress I didn't have the time to create something that would be meaningful to scientists. My interviewees, though, had made comments about where this could be shown: "this is like an aquarium exhibit."

From then on, I designed my website as if it was going to be shown at the Monterey Bay Aquarium. I kept the approachable, inviting tone while retaining the scientific background that makes the topic so interesting. Although I lament the time I lost after my motherboard went for a swim, I think it came with a silver lining. The time crunch forced my visualizations to be simpler. I had to ask myself "what is the least time-consuming way I can convey my message to my audiecne, without having to piece together a bunch of disparate data sets?" In the end, this enhanced the website's connection with its target audience.

It also made my call to action more straightforward. If my target audience was aquarium-goers, then I had to limit my call to action to things that ordinary people actually had the power to do. Donating to the Monterey Bay Aquarium was a no-brainer since they are a primary contributor of funding for researching this topic. However, just donating didn't seem active enough for me. In my research, I encountered an organization called Reef Check. They train people to scuba dive and launch expeditions of citizen scientists to directly help maintain kelp forests, including cleaning up sea urchin barrens. It seemed like a perfect fit--now there were two tiers from which people could choose. The first is for anybody who cared about the kelp forest ecosystem, and the second is for those who are willing to get their hands dirty and help preserve kelp forests firsthand.

In the end, while I couldn't do everything I had wanted to, I created a website that, I think, does a good job of telling a story for people interested in the topic and giving them a chance to act. And who knows, maybe I will revisit this project in the future and make the website I initially wanted to create.

[Back to Portfolio](README.md)
