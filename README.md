# Data-Visualization
https://plotly.com/python/choropleth-maps/
## 1. Data Overview
### 1.1. Collumns:
+ 'ID': Unique ID of each athelete. Different atheletes can participate in several events
+ 'Name': Name of atheletes. Example: 'Lionel Hunter Escombe'
+ 'Sex': Gender: 'M' or 'F'
+ 'Age': Age of that athelete when participate, Integer
+ 'Height': Height of that athelete when participate, Integer
+ 'Weight': Weight of that athelete when participate, Integer
+ 'Team': Team name that athelete was in, some country has more than 1 team.
+ 'NOC': National Olympic Committee 3-letter code
+ 'Games': Year and season. Example: '1904 Summer'
+ 'Year': Year
+ 'Season': Summer or Winter
+ 'City': Host city of Olympics. Example: 'St. Louis'
+ 'Sport': Sport, example: 'Athletics'
+ 'Event': Specific event that athelete join. Example: 'Athletics Men's Marathon'
+ 'Medal': Medal.
### 1.2. Overview graphs on each attributes and on whole data (HƯNG)
+ On Sex: Vertical bars of 2 genders, and maybe over years/decades, or different plots for each year and concanate to interactive or gif (mainly to show the evolution of height/weight of atheletes over years)
+ On Age: Pie chart with relative size to show the distribution of age and total number of participants over years/decades
+ On Height and Weight: Scatter plot by years/decades (could use different colors for each year/decade), or different scatter plots for each year and concanate to interactive or gif (mainly to show the evolution of height/weight of atheletes over years)
+ On NOC: Use map and if possible, maps over years/decades of participated country/region
+ On Medal: Number of medal overyears.
## 2. Write down questions to explore:
Which information can we retrieve from our data? 
Which advanced problems can be inferred ?
Which data need to be involved ?
### 2.1. Which continents are dominating which sport field Olympics over decades ? (NHẬT)
+ Data involved: 
  + (external) countries on continents, NOC groupby continents (Remember to check integrity constraint) (DONE)
    + https://stillmed.olympics.com/media/Document%20Library/OlympicOrg/Documents/National-Olympic-Committees/List-of-National-Olympic-Committees-in-IOC-Protocol-Order.pdf
    + Tools: https://py-pdf-parser.readthedocs.io/en/latest/index.html
  + Medals groupby NOC over Years/Decades, Medals by sports by continents by years/decades 
  + Count Atheletes per continents by sports over years/decades
  + Medals/Atheletes Ratio by continents by sports over Years/decades
+ Graphs to show:
  + Mainly interactive map, maps and mapssss with bar chart on it: Maps for summary (i.e. All-time olympic dominating country/continent)
    + https://datavizproject.com/data-type/map-bar-chart/
    + https://datavizproject.com/family/geospatial/
  + OR use gif to show the change of ranking by decades: (take a look at https://www.youtube.com/watch?v=eP88FUL7d_8&ab_channel=DataIsBeautiful for example)
    + https://towardsdatascience.com/creating-beautiful-gif-with-python-for-your-data-analysis-ac50c618b559 
### 2.2. Which region/country lead the achievement of which continent ? (LẬP)
For each dominating continent on some interested sports, we take a look deeper to find out which countries are the strongest of that continent.
+ Data involved:
  + Medals groupby countries over years/decades and continents for color coded
  + Maybe extracted informations for some specific sports (football, athletics, swimming...)
+ Graphs to show:
  + Gif of ranking in countries' medals, color coded by continents
    + ![image](https://user-images.githubusercontent.com/72718669/167535367-c9bc3ff2-d262-4ef5-8c8f-274f0d3a70ad.png)
### 2.3. Sex distribution over years, over regions and sports -> the evolution of Gender awareness affects to Olympics (TRƯỜNG)
+ Data involved:
  + Athletes count groupby gender by years/decades, can be encoded by sports or continents
+ Graphs to show:
  + Can be a gif of pie chart with 2 portions of male/female, show changes over time of distribution
    + https://www.reddit.com/r/dataisbeautiful/comments/ulamcb/oc_worldwide_coffee_production/
  + Plot the difference of male - female on some sports over years
-> the evolution of gender awareness
### 2.4. "Sports are neutral to politics" -> During World's recent conflict (i.e Gaza, Taliban, Middle East, Iran, Iraq, and most reecently: Ukraine)
### 2.5. Some fun facts about Olympics: oldest, youngest, etc... (HƯNG)
+ 
