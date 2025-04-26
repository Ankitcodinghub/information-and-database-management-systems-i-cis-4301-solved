# information-and-database-management-systems-i-cis-4301-solved
**TO GET THIS SOLUTION VISIT:** [Information and Database Management Systems I (CIS 4301) Solved](https://www.ankitcodinghub.com/product/information-and-database-management-systems-i-cis-4301-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;102319&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Information and Database Management Systems I  (CIS 4301) Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
<h1>Question 1 (SQL Queries)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; [85 points]</h1>
We are given a geostatistical database about countries, continents, rivers, etc. The following information is available in Canvas together with data for download:

<ul>
<li>An ER diagram of the geostatistical database in PDF format (<em>HW3Ex1- geostatistical-database-ERdiagram.pdf</em>).</li>
<li>An informal description of the database schema in PDF format (<em>HW3Ex1- geostatistical-databaseschema-explanation.pdf</em>).</li>
<li>A text file that contains create table commands to create the database schema (<em>HW3Ex1-geostatisticaldatabase-schema.sql</em>).</li>
<li>A text file hat contains insert commands for about 47,800 tuples to fill the database tables (<em>HW3Ex1geostatistical-database-input-data.sql</em>).</li>
<li>A text file that contains drop table commands to delete the database schema and the data in the database (<em>HW3Ex1-geostatistical-database-drop-tables.sql</em>).</li>
</ul>
Use the CISE Oracle DBMS and the Oracle SQL Developer software to create the database schema and fill the database with data. This will also help you learn about the system environment for your group project. In particular, the use of MySQL, PostgreSQL, and other database systems is not allowed.

(a) [10 points] Look at the database schema in the file <em>HW3Ex1-geostatistical-database- schema.sql</em>. You will find the following SQL statements from line 38 to line 52:

ALTER TABLE Country

ADD CONSTRAINT FK_CountryREFCity

FOREIGN KEY (Code, Capital, Province)

REFERENCES City(Country, Name, Province)

INITIALLY DEFERRED DEFERRABLE;

ALTER TABLE City

ADD CONSTRAINT FK_CityREFProvince

FOREIGN KEY (Country, Province)

REFERENCES Province(Country, Name)

INITIALLY DEFERRED DEFERRABLE;

ALTER TABLE Province

ADD CONSTRAINT FK_ProvinceREFCountry

FOREIGN KEY (Country)

REFERENCES Country(Code)

INITIALLY DEFERRED DEFERRABLE;

ALTER TABLE Province

ADD CONSTRAINT FK_ProvinceREFCity

FOREIGN KEY (Capital, Country, CapProv)

REFERENCES City(Name, Country, Province)

INITIALLY DEFERRED DEFERRABLE;

Your task is to explore this scenario by using the Internet. The keywords INITIALLY DEFERRED DEFERRABLE are non-standard SQL. They are supported by several database systems such as Oracle and PostgreSQL.

Answer the following questions.

<ul>
<li>[4 points] What is the meaning of these keywords?</li>
<li>[6 points] Why is the action indicated by the keyword INITIALLY DEFERRED DEFERRABLE needed in the scenario above? What is the problem? How is the problem solved?</li>
</ul>
(b) [75 points] Write SQL queries for the colloquial queries below and show the results by providing screenshots for both your SQL queries and query results. The screenshots must be embedded into the PDF file that contains your solutions to this whole assignment. In order to increase readability, the SQL queries should be written in a structured manner, all SQL keywords should be fully capitalized, and the table and attribute names should be written in the same way as in the schema file.

If not explicitly forbidden, the use of the Oracle specific “row limiting functions” such as the “FETCH” clause and the “ROWNUM” function is allowed. The following two examples illustrate their use:

SELECT &lt;column_name(s)&gt;

FROM &lt;table_name&gt;

ORDER BY &lt;column_name(s)&gt;

FETCH FIRST &lt;number_of_rows&gt; ROWS ONLY;

SELECT &lt;column_name(s)&gt;

FROM &lt;table_name&gt;

ORDER BY &lt;column_name(s)&gt;

WHERE ROWNUM &lt;= &lt;number_of_rows&gt;;

Write SQL queries for the following questions and provide screenshots as described above.

<ul>
<li>[3 points] What is the largest city in terms of population for each continent? Show the continent name, city name, and city population. Order the result by population in descending order.</li>
<li>[3 points] What are the countries and provinces in each continent with the highest population density? Population density is expressed as the number of people per unit area. Display the names of the countries, provinces, and continents as well as the population density.</li>
<li>[3 points] Find the names of provinces in Europe that have more than two lakes, each with an area less than 500 square kilometers.</li>
<li>[3 points] Find the provinces that have an island of type ”volcanic”. List the province name, the number of islands of type ”volcanic”, and the total area of these islands in each province. Order the results by the total area in descending order. Exclude a result if the total area is null. Display only the top three tuples.</li>
<li>[2 points] What are the names and elevations of the highest mountain of each type? Display the mountain names, elevations, and types together and order by ascending elevation. Do not include the mountains with a null type.</li>
<li>[4 points] What are the top 10 countries with the longest total border length, and what is the length of each country’s border? Find the names of countries and length of borders together.</li>
<li>[2 points] What is the total population of Muslim in Europe?</li>
<li>[3 points] Find the names of cities that have more than two airports and where the city is located in a province with a population greater than 1 million and the province is in Europe.</li>
<li>[3 points] Which countries have a GDP higher than the average GDP of the top 10 European countries. Display the names of countries and the respective GDPs of those countries, ordered by GDP in descending order.</li>
<li>[4 points] Find the names of countries where Spanish and English are spoken and the population of people speaking Spanish is larger than the population of people speaking English. Show the names of the countries and the populations of people speaking Spanish and English.</li>
<li>[5 points] Which countries among the countries whose GDP is higher than 2.2 million have a higher or lower inflation and a higher or lower unemployment rate compared to the average rate of their respective continent? Display the name of the continent, the name of the country, the difference in inflation, and the difference in unemployment for each country, ordered by continent.</li>
<li>[3 points] What are the names of the seas that touch the largest number of provinces? For this question, do not use “row limiting functions” such as the “ROWNUM” function or the “FETCH” clause.</li>
<li>[3 points] What are the names of the countries where the proportion of Christians is greater than the proportion of Muslims? Exclude the countries where either religion is not present.</li>
<li>[3 points] Find the countries that have at least 3 islands and that have a sea or seas with a total area greater than 35,000,000 km<sup>2</sup>. List the names of those countries along with the number of islands and the area of the sea(s). Order your result by the number of islands in ascending order.</li>
<li>[3 points] What is the name of the country that has the highest GDP per capita? Display the name of the country along with the GDP per capita.</li>
<li>[3 points] What are the names of the seas that are adjacent to the country that has the city with the highest latitude?</li>
<li>[4 points] Which seas have the maximum or minimum number of islands, and what is the number of islands in those seas?</li>
<li>[3 points] Find all seas that are bordered by more than 5 countries and have an average depth greater than 300 meters. Display the number of countries bordering a sea along with the names and average depths of these seas. Order the result by the number of countries bordering a sea in descending order.</li>
<li>[3 points] How many deserts are there in African provinces with a population greater than 10 million?</li>
<li>[3 points] What are the names and the elevations of the top 10 highest mountains located on islands in Asia?</li>
<li>[3 points] What are the names of the provinces that have a population greater than 10 million and are located in a country that is a member of the European Union? Do not hard-code the abbreviation ’EU’. Display the results in a table showing the names of the provinces, their populations, and the names of the countries they are located in.</li>
<li>[4 points] What are the names of the provinces and lakes in Europe with a population density greater than 100 and where the average lake depth is less than the average lake depth in Europe?</li>
<li>[2 points] Identify the provinces with mountains of type ’volcano’, the number of ’volcano’ mountains in each province, and the total population of each province. Present the information as follows: province name, number of mountains, and total population. Only consider provinces with a population greater than 10,000,000 and sort the results in ascending order of population.</li>
<li>[3 points] What is the most widely distributed ethnic group in the world, and in how many countries can it be found? Show the name of the ethnic group and the number of countries it is located in.</li>
</ul>
<h1>Question 2 (SQL and Relational Algebra)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; [6 points]</h1>
For the following SQL statement, give an equivalent Relational Algebra expression if possible. If such an expression cannot be given, explain why.

SELECT DISTINCT enum

FROM&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; employee

WHERE&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; NOT EXISTS

(

SELECT *

FROM&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; projects

WHERE NOT EXISTS

(

<h2>SELECT *</h2>
FROM&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; works

WHERE employee.enum = works.enum AND works.pnum = projects.pnum

) );

<h1>Question 3 (QBE)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; [9 points]</h1>
Consider the following table schemas (primary keys are underlined):

<ul>
<li>Company(<u>cID</u>, name, location)</li>
<li>Flight(<u>cID</u>, <u>fnumber</u>, departure, arrival, price:integer, number of seats: integer)</li>
<li>Book(<u>bID</u>, cID, fnumber, customerID, seat, date)</li>
<li>Customers(<u>customerID</u>, name, address)</li>
</ul>
Draw Query-by-Example (QBE) tables for the following queries.

<ul>
<li>[3 points] Find the names and addresses of customers who never booked a flight.</li>
<li>[3 points] Find the names of customers who booked flights to Boston and Seattle.</li>
<li>[3 points] Insert tuples into a new table <em>CustomerCheck </em>that stores the names and addresses of customers who booked a flight from New York to LA on 04/30/22 and also provides their flight numbers.</li>
</ul>
