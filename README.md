<h1>Car-Details</h1>
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="">Business Understanding</a>
      <ul>
        <li><a href="">Scope</a></li>
      </ul>
    </li>
    <li>
      <a href="">Data Understanding</a>
      <ul>
        <li><a href="">Data Source</a></li>
        <li><a href="">Variables of Interest</a></li>
        <li><a href="">Data Types</a></li>
        <li><a href="">Visualisation Requirements</a></li>
        <li><a href="">Comparative Analysis</a></li>
      <a href="">Approach</a>
    </li>
    <li>
      <a href="">Visualisations</a>
    </li>
    <li>
      <a href="">Interpretations</a>
    </li>
    <li>
      <a href="">Technologies</a>
    </li>
    <li>
      <a href="">Setup</a>
    </li>
    <li>
      <a href="">Status</a>
    </li>
    <li>
      <a href="">Credits</a>
    </li>
  </ol>
</details>
<P>The main goal of this project is to answer the questions "".</P>

<h2>Business Understanding</h2>

<h3>Scope</h3>
<p>This analysis takes place between 2010 and 2020.</p>

**Credibility Criteria**  
<p> The Bigfoot sightings were classified into 3 report types:

 </p> 

<p> In this analysis I consider --- to be credible if...</p>

<H2>Data Understanding</H2>
<h3>Data source</h3>
<p>The data source I am using is the  Excel file which I obtained through my Introduction to Tableau module in my Data Analytics Essentials course.

I believe this data to be reliable because firstly, the data was sourced from <a href=https://www.bfro.net/GDB/#usa>WWW.BFRO.NET</a> which is the only scientific research organization exploring the bigfoot/sasquatch mystery. The data used in my analysis is from their comprehensive database of credible sightings and related reports which is maintained by an all-volunteer network of bigfoot/sasquatch researchers, archivists, and investigators in the United States and Canada.
</p>

<h3>Variables of Interest</h3>
<p> The key variables I want to analyse within this project are as follows:
<ol>
  <li>Number of sightings</li>
  <li>States in which sightings occured</li>
  <li>Counties in which sightings occured</li>
</ol>
</p>

<h3>Data Types</h3>
<p>My data contains:
  <ul>
    <li>Report Type - String</li>
    <li>Report Class - String</li>
    <li>Submitted Date - Date and Time</li>
    <li>Year - String</li>
    <li>Season - String</li>
    <li>Month - Date and Time</li>
    <li>State - String</li>
    <li>County - String</li>
  </ul>
</p>

<h3>Visualisation Requirements</h3> 
<p>I want to first use a horizontal bar chart in order to visualise the state with the most sightings. Then I want to use a symbol map in order to visualise which counties within the selected state had the most sightings.</p>

<h3>Comparative Analysis</h3>  
<p> I want to compare sightings within the selected state in 3 different ways: 
<ol>
  <li>The season in which reports were made</li>
  <li>The month in which reports were made </li>
  <li>The class types of reports made</li>
</ol>

In order to identify any patterns or trends with when these reports were made.</p>

<H2>Approach</H2>

<h3>Data Collection</h3>
<p>To collect the data used for this analysis I downloaded an Excel file within the Cisco 'Introduction to Tableau module' in my Data Analytics Essentials course.</p>

<h3>Data Cleaning</h3>
<p>First I put a filter on the entire date in order to make the cleaning process easier, I then removed the 'Submitted Date' column as this was irrelevant to my analysis. Then I used conditional formatting on the year column to highlight any data rows outside the range of 1950 - 2018. After this, I filtered all the class C reports and removed them from the dataset as they were not deemed credible enough for the analysis. I then filtered all the 'unknown' cells in the 'Season' column and removed these rows of data as they would've affected my comparative analysis later during the project, I also filtered all the '(blanks)' cells in the month column in order to remove the lines of data that didn't have a specific month as these lines of data would affect my upcoming comparative analysis.</p>

<h3>Analysis</h3>  
<p>Using a pivot table I put the state column in the row and values fields and then I sorted the data descending by 'Count of State' which showed me that Washington had the highest number of sightings (506).</p>

<p>I then created a second pivot table. This time I put 'State' and then 'County' in the Rows field and then I put 'Count of County' in the Values field in order to show sightings per county. I then sorted the data descending by 'Count of County', and then I filtered on the state of Washington in the Row field, as this was the state with the most sightings, which showed me that 'Pierce' was the county with the most sightings.</p>  



<h2>Visualisations</h2>
<a href="https://public.tableau.com/app/profile/deiniol.ampomah/viz/BigfootSightings_16995777430520/BigfootSightings1"> <img src="https://github.com/DkOwusuA004/Bigfoot-Sightings/blob/main/Bigfoot%20sightings%20by%20State%20&%20Washington%20sightings%20by%20County%20Dashboard.png?raw=true45f3179c-c7c2-4acd-a123-a800a1676d0c" alt="Bigfoot Sightings Dashboard 1">
</a>

<a href="https://public.tableau.com/app/profile/deiniol.ampomah/viz/BigfootSightings2/BigfootSightings2"><img src="https://github.com/DkOwusuA004/Bigfoot-Sightings/blob/main/Washigton%20sightings%20by%20Season,%20Class%20&%20Month%20Dashboard.png" alt="Bigfoot Sightings Dashboard 2"></a>




<h2>Interpretation</h2>
<p>Within the first dashboard are 2 graphs; 'Bigfoot sightings by State' and 'Washington sightings by County'. The 'Bigfoot sightings by State' shows us that Washington produced the most Bigfoot sightings (503) between 1950-2018. This answers the first question "Which state within the USA had the most sightings over the period?".</p>

<p>In order to answer the second question; "Within this state which county was responsible for the majority of these sightings?", we have to look at the 'Washington sightings by County' graph. This graph shows us that within Washington, the county with the highest number of sightings is Pierce County with 68 sightings in the period.</p>

<p>Regarding the comparative analysis we can look at tables 'Sightings by season', 'Sightings by month' and Sightings by class'.</p>

<p>Firstly, by looking at the 'Sightings by season' graph, we can see that 40.36% of sightings (203) were reported during Summer, this could be due to the following:
  <ol>
    <li>Increased Outdoor Activity</li>
    <p>During the summer season, a pronounced surge in vacationing and recreational pursuits is observed. Many individuals, particularly outdoor enthusiasts such as campers and hikers, tend to partake in these activities during this period, capitalizing on the more predictable weather conditions. This propensity raises the probability of individuals finding themselves in locations where reported Bigfoot sightings have historically occurred. Furthermore, the summer months represent an optimal time for wildlife observation. Devotees of nature and photography often allocate an increased duration to exploring natural habitats, thereby augmenting the chances of encountering diverse fauna. It is noteworthy that such wildlife encounters, in certain instances, may be misconstrued as potential Bigfoot sightings.</p>
    <li>Better Weather Conditions/Extended Daylight Hours</li>
    <p>The elevated temperatures of the summer season render outdoor activities notably more comfortable and enticing. Consequently, individuals are inclined to explore natural habitats, thereby heightening the prospects of wildlife encounters or reporting unconventional sightings. Moreover, the longer duration of daylight during summer extends the time available for outdoor activities. This prolonged visibility window creates additional opportunities for individuals to discern peculiar phenomena and subsequently report such sightings.</p>
    <li>Wildlife Activity/Migration and Movement Patterns</li>
    <p>In the summer season, numerous wildlife species undergo heightened activity, influenced by factors like breeding seasons, abundant food availability, and favourable weather conditions. This surge in wildlife activity is prone to result in increased observations and reports from individuals engaged in outdoor activities, particularly in regions recognised for Bigfoot sightings. Furthermore, locales characterised by both documented Bigfoot sightings and escalated wildlife activity may witness elevated instances of human-wildlife interactions. This heightened interaction dynamic amplifies the likelihood of individuals reporting sightings, contributing to the convergence of reported encounters in these areas.</p>
  </ol>
</p>

<p>Next, looking at the 'sightings by month' graph, we can see that the month of August had 88 sightings reported out of a possible 503 (11.73%). This graph shows us that the summer sightings were greatly influenced by the month of August as the 2nd and 3rd highest months after August were October (68) and September (67) </p>

<p>Finally, the 'sightings by class' graph shows that the majority (58.65%) of reports made were reports involving incidents where a possible sighting was observed at a great distance or in poor lighting conditions </p>

<h2>Potential Biases</h2>
<p>The most prevalent type of bias that could've affected the conclusion of this project is information bias; many people may have had sightings that could very well fall under Class A or B reports however, for an array of reasons they may not have filed a report. In addition to this, there is the risk of hoax and prank reporting which affects the validity of the data collected, ultimately skewing the data and creating inaccuracies within the analysis. </p>


<h2>Technologies</h2>
<img src="https://download.logo.wine/logo/Microsoft_Excel/Microsoft_Excel-Logo.wine.png" alt="Excel Logo" width="150" height="100">

<img src="https://1000logos.net/wp-content/uploads/2022/03/Tableau-Logo.png" alt="Tableau Public Logo" Width="150" height="80">

<h2>Status</h2>
<p><img src="https://geps.dev/progress/100"></p>


<h2>Credits</h2>
<a href="https://www.kaggle.com/datasets/josephvm/bigfoot-sightings-data">Bigfoot Sightings</a>
