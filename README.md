# DV_PROJECT_FALL2017
The Visualization are  developed as part of the UIUC-DV590-FAll2017 project. 

## For execution of the code the below pre-requisite are needed. 
1. Install [bqplot](https://github.com/bloomberg/bqplot). 
2. Once installed, copy the TransportableArrMap.json into "Anaconda3\Lib\site-packages\bqplot\map_data"
3. Download all the datasets in the 'data' folder 

## Group name: 
the PAJTplotters

## Group members: 
Pratik Shrivastava, Thuong Phan, Yi-Yun Cheng (Jessica), Yuejun Wu (Amber) 

## Our Approach:
### The use of bqplot library
- Strength

The bqplot gave us a straightforward and easy way to implement code, specifically, the interactive part between the different bqplot elements (such as map and line plot) can be incoprated and integrated with ease. In our approach, we also implementend ipywidgets to provide more appealing visual cues. 

- Weakness/ Problems we encounter

The interactivity required additional callback functions - which may lead to potentional(unknown) errors. The interlinking parameters of multiple functions made it harder for us to detect the errors. 
The plotting of points on the map required additional programming. Originally, using only the USStatesMap.json to plot the points made the plot static and would not change to fit the scale when we adjust or zoom in on the map. A customized json file (thanks to the other group's help) for US state map "TransportableArrMap.json" is required to solve the problem.

### The interative hovering tooltip
We used the annotate() method in matplotlib to create tooltip, there're also some strengths and weaknesses:

- Strength 

It is flexible, we can add as many data into the tooltip as we want. In addition, we can also customize the shape, color and arrowprops for tooltip. 

- Weakness

To make the tooltip become interative, we need to change the backend to matplotlib nbagg, and also requires additional event handling programming codes. The "event handling" in matplotlib uses mpl_connect() method for "motion_notify_event" and create a separate method for hovering event handling.


## Refrences
### for the codes

- https://stackoverflow.com/questions/47242637/why-doesnt-imshow-show-pixel-values-when-i-hover-over-it
- https://stackoverflow.com/questions/27704490/interactive-pixel-information-of-an-image-in-python
- https://github.com/bloomberg/bqplot
- https://matplotlib.org/examples/color/colormaps_reference.html
- http://ipywidgets.readthedocs.io/en/stable/examples/Widget%20List.html?highlight=PLAY

### for the infographic

- https://history.nasa.gov/40thann/define.htm
- http://www.nuforc.org/index.html
- http://www.thepeoplehistory.com/1990.html
- https://www.onthisday.com/date/1990
- https://www.economist.com/news/united-states/21605918-everything-you-need-know-about-ufos-0
- https://www.theatlantic.com/technology/archive/2014/06/the-hard-data-on-ufo-sightings-its-mostly-drunk-people-in-the-west/373645/
- http://www.imdb.com/list/ls000095891/
- https://auxiliarymemory.com/2013/05/02/the-defining-science-fiction-books-of-the-1990s/
- http://bestsciencefictionbooks.com/blog/10-essential-sf-books-of-the-1990s/


## Contributions
### Component 1: 
#### Map & Line plot
- Pratik Shrivastava: code (Map, line plot and time slider); research on bqplot and other packages to do interactive graphics on Map, line plot, time slider; data management; data cleaning; writeup 
- Yuejun Wu (Amber): data cleaning; code (Map) 

#### Spectrogram

- Thuong Phan: code (data normalization, interactive graphics); data management; data cleaning
- Yi-Yun Cheng (Jessica): research on the interactive backends & hovering; markdown notes

### Component 2:
- Pratik Shrivastava

### Component 3:
- Thuong Phan: data processing, data normalization, data extraction, basic interaction graphics
- Pratik Shrivastava: interactive graphics

### Component 4:
- Yi-Yun Cheng (Jessica): data management; create and design the infographics using Canva; research on UFOs and the meaning of the codes (e.g. reading up the articles from the reference listed above)
- Yuejun Wu (Amber): data management; research on the meaning of the codes; help Jessica on infographics design

### Final write-up: 
Everyone
