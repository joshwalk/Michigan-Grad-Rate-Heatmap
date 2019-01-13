# Michigan High School Graduation Heatmap

![app screenshot](https://raw.githubusercontent.com/joshwalk/MIGraduationMap/master/fullMI.jpg)
![app screenshot](https://raw.githubusercontent.com/joshwalk/MIGraduationMap/master/southeastMI.jpg)

My project involves visualizing the 2017 4-year graduation rates of all public high schools in the state of Michigan by location. In a sociology class I took last year, we discussed the reasons and implications behind high/low graduation rates. I wanted to analyze this at a state level (with a particular focus on the metro Detroit area) to determine any concentration of successful/unsuccessful high schools. There are a couple questions I wanted to answer:
- Where are the most notable areas that exhibit a large disparity in graduation rates?
- Are schools that have very high or very low graduation rates isolated to certain geographical areas? Or spread somewhat evenly across the state?

## Data Sources
- 2017 Michigan Graduation/Dropout Rate by District and School
- Google Places API Text Search Service​, using request URLs containing queries of school name, county, and state

## Analysis
For my analysis and visualization I used ​OpenHeatMap​. I converted my final dataframe to a CSV file that was imported through the OpenHeatMap webapp. I used a scale of 35-100% and used traditional “heat” colors on a scale of red, yellow, and green; red represented the lowest rates and green the highest. The Upper Peninsula is sparsely populated so I focused on analysis of the Lower Peninsula.

Overall, the graduation rates seem spread fairly evenly across the state. I adjusted the “blob size” until I was able to make note of distinct areas of low performing schools. Of these, I determined the area known as ​downriver Detroit​ to be the worst, followed by Ludington/Manistee and Charlevoix/Petosky.

I am from southeastern Michigan so I was interested in analyzing the map of the metro Detroit area specifically, which happens to also be the highest concentration of high schools in the state.

There are many more red areas than I would have expected. My hypothesis was that the city limits of Detroit would be red/yellow and the surrounding areas green. There are many “pockets” of dark red surrounded by bright green, corresponding to very low and very high graduation rates. There is a large disparity in graduation rates in many areas throughout Detroit and its near suburbs.

My hypothesis was based on my own knowledge and perception of the wealth of communities in SE Michigan, and while some of the results were surprising, other confirmed my guesses. In the areas northwest of Detroit (like Farmington Hills, West Bloomfield, Novi, Northville) graduation rates are consistently very high.

There is a pitfall in the generation of the heat map that I noticed upon close inspection. I discovered that some small, alternative schools have very low graduation rates and that this can misrepresent the rest of the area immediately surrounding it. I don’t believe this significantly altered the results but it is certainly occasionally present.

Overall, I found this project to be very interesting and I was surprised by some of the results. I was able to identify and analyze a number of areas in Michigan with clusters of low performing high schools. I believe this visualization could be useful for the Michigan Department of Education to determine key areas where action could be taken at a level other than school or district-specific.