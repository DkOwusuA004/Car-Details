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
<P>The main goal of this project is to answer the following questions; "Which manufacturers were top based on the number of cars sold?", "What was the most purchased transmission?" and "Which manufacturers were top based on the total selling price of cars sold?".</P>

<h2>Business Understanding</h2>

<h3>Scope</h3>
<p>This analysis takes place between 2010 and 2020.</p>

**Credibility Criteria**  
<p> The cars were classified into 4 fuel types:
     
  - Petrol
  - Diesel
  - LPG
  - & CNG

 </p> 

<p> In this analysis I consider car sales to be credible if they were either petrol or diesel cars</p>

<H2>Data Understanding</H2>
<h3>Data source</h3>
<p>The data source I am using is the  Excel file which I obtained through the database website <a href="https://www.kaggle.com/datasets/akshaydattatraykhare/car-details-dataset/data">Kaggle.</a>

I believe this data to be reliable because firstly, the data was sourced from <a href="https://www.cardekho.com/">www.cardekho.com</a> which is India's leading car search venture that helps users buy cars that are right for them. Its website and app carry rich automotive content such as expert reviews, detailed specs and prices, comparisons and videos/pictures of all car brands and models available in India. A bunch of young, enthusiastic IT graduates set up the website. Its investors include Google Capital, Tybourne Capital, Hillhouse Capital, Sequoia Capital, HDFC Bank, Ratan Tata and Times Internet.
</p>

<h3>Variables of Interest</h3>
<p> The key variables I want to analyse within this project are as follows:
<ol>
  <li>Number of cars sold per manufacturer</li>
  <li>Value of total cars sold per manufacturer</li>
  <li>Number of cars sold per transmission</li>
</ol>
</p>

<h3>Data Types</h3>
<p>My data contains:
  <ul>
    <li>Manufacturer - String</li>
    <li>Model- String</li>
    <li>Year - String</li>
    <li>Selling Price - Floating Pointing</li>
    <li>Km Driven - Integer</li>
    <li>Transmission - String</li>
    <li>Owner - String</li>
    <li>Engine - Floating Pointing</li>
    <li>Seats - Integer</li>
  </ul>
</p>

<h3>Visualisation Requirements</h3> 
<p>I want to first use a bar chart to visualise the manufacturers with the most number of cars sold. Then I want to use a treemap to visualise which suppliers generated the most in selling price. Finally, I used a pie chart to show the split between manual and automatic transmission.</p>


<H2>Approach</H2>

<h3>Data Collection</h3>
<p>To collect the data used for this analysis I downloaded an Excel file from the Kaggle website from a dataset called <a href="https://www.kaggle.com/datasets/akshaydattatraykhare/car-details-dataset/data">"Car Details Dataset"</a>.</p>

<h3>Data Cleaning</h3>
<p> First I added a filter on the data which would allow me to easily spot unique values within columns. I then converted the selling price and Km-driven columns to numbers and used =COUNTBLANK in column N with a range of A:M to locate any rows with blank cells. Once I had located these blank cells I removed those rows of data to ensure I had the most information possible when creating my visualisations. I then added 2 columns before column B and used =LEFT(A2,FIND(" ",A2)) in cell B2 to pull through the manufacturer name from the Name column, I also used =MID(A2,LEN(B2)+1,LEN(A2)-LEN(B2)) to pull through model. I dragged these formulas down so that they covered the entire dataset. After this, I filtered on years before 2010 and deleted them as my scope was 2010-2020. I also removed fuel types that weren't either petrol or diesel because petrol and diesel cars have historically dominated the automotive market. Analysing these types provides a comprehensive understanding of the majority of vehicles on the road, making my analysis relevant to a larger audience. I then removed the rows relating to test-driven cars as I only wanted to include cars that were sold.
</p>

<h3>Analysis</h3>  
<p>Using a pivot table I put the manufacturer in the row and put the count of manufacturers and the sum of selling price in the values fields. Using the MAX and Min formulas I pulled through the max and min count of manufacturers and the sum of the selling price which showed me that Maruti had the highest number of cars sold (1902) with the highest total selling price (899,623,919.00 rupees) and Ashok sold the least amount of cars (1) with the lowest total selling price (300,000.00 rupees).</p>

<h2>Visualisations</h2>
<a href="https://public.tableau.com/app/profile/deiniol.ampomah/viz/CarDetails_17084697056090/Dashboard1"> <img src="https://github.com/DkOwusuA004/Car-Details/assets/139594033/709584e2-e96b-4b96-985a-70ee4e95a6ca" alt="Car Details Dashboard 1">
</a>



<h2>Interpretation</h2>
<p>Within the dashboard are 3 graphs; 'Number of cars sold by Manufacturer', 'Manual vs Automatic Transmission' and 'Total selling price by Manufacturer'. The 'Number of cars sold by Manufacturer' shows us that Maruti sold the most cars  (1,902). This answers the first question "Which manufacturers were top based on the number of cars sold?".</p>

<p>In order to answer the second question; "What was the most purchased transmission?", we have to look at the 'Manual vs Automatic Transmission' graph. This graph shows us that out of the 6,875 cars sold, the majority of those cars (86%) were manual transmission while only 14% were automatic transmission.</p>


<P>To answer the final question; "Which manufacturers were top based on the total selling price of cars sold?", we can use the 'Total selling price by Manufacturer' graph. This graph shows us that the manufacturer Maruti had the highest total selling price (899.62 million rupees).</P>

<p>Firstly, by looking at the 'Number of cars sold by Manufacturer' we can see that Maruti; an Indian subsidiary of Japanese automaker Suzuki sold the majority of cars during the period. The reasons for this could be the following...
<ol>
  <li>Affordability and Value for Money</li>
  <P>Maruti Suzuki offers a wide range of cars that cater to various price segments, providing value for money with competitive pricing, fuel efficiency, and low maintenance costs. This makes their cars attractive to a broad demographic.</P>
  
  <li>Strong Brand Loyalty and Trust</li>
  <p>Over the years, Maruti Suzuki has built a strong reputation for reliability and trustworthiness. Many Indian families have owned Maruti cars for generations, fostering brand loyalty.</P>

  <li>Efficient After-Sales Service</li>
  <p>Maruti Suzuki’s extensive service network ensures that customers have easy access to maintenance and repairs. The availability of spare parts at affordable prices further enhances customer satisfaction.</P>
  
  <li>Government and Regulatory Support</li>
  <p>Maruti Suzuki has benefited from favourable government policies and regulations, including initiatives promoting the manufacturing sector and incentives for small cars, which form a significant part of their lineup.</P>
  
  <li>Local Manufacturing and R&D</li>
  <p>Maruti Suzuki's strong local manufacturing presence and investment in research and development allow them to produce cars tailored to Indian conditions and preferences, ensuring competitive pricing and better market acceptance.</P>
</ol>

<p>These above factors collectively give Maruti Suzuki a significant edge over its competitors in the Indian automotive market.</p>
</p>



<h2>Technologies</h2>
<img src="https://download.logo.wine/logo/Microsoft_Excel/Microsoft_Excel-Logo.wine.png" alt="Excel Logo" width="150" height="100">

<img src="https://1000logos.net/wp-content/uploads/2022/03/Tableau-Logo.png" alt="Tableau Public Logo" Width="150" height="80">

<h2>Status</h2>
<p><img src="https://geps.dev/progress/100"></p>


<h2>Credits</h2>
<a href="https://www.kaggle.com/datasets/josephvm/bigfoot-sightings-data">Car Details Dataset</a>
