# fec.md
# MARKDOWN DATA DIARY 
## Ananya Tiwari
### LINK: https://docs.google.com/spreadsheets/d/1kEIM1GznidgTrdZwM1hn1JI7IWoViUvhpfQuvY6mj58/edit#gid=252747239 
<br>
1. I opened the Dataset on OpenRefine <br><br>
2. I opened the text facet for Donor column, to see how it is formatted. <br><br>
3. I realized that the donor list comprised of lots of organizations/industries as well as individuals. I also realized that certain entities donated money more than 2 times: <br><br>
* Philip Morris 13 <br>
* American Fedn of St/Cnty/Munic Employees 7 <br>
* Revlon Group Inc 6 <br>
* Senate Republican Campaign Cmte 6 <br>
<br>
4. When I opened the text facet for the column Amount, it realized that most donations (320) are $100,000 lump sum donations, followed by 17 $250,000 sum donations, and 14 $150,000 donations. 
<br><br>
5. Opening the text facet for the Party column (with R and D), I realized that three donations were given to a party named “3”, which I saw meant the “Natural Law Party of the United States”. Republicans got 213 donations, and Democrats 185. 
<br><br>
6. After opening text fact for Sector, I saw that 15 of them were “Unknown”, and 6 were “Other”, and 67 were under “Misc Business”. I decided to club them all under Misc Business. 
<br><br>
7. Opening the text facet for Industry, I renamed Misc Unions to Workers’ Unions, A lot of corporations were also under Category Unknown. 
<br><br>
8. Text facet of City revealed that most of the donors came from New York (72), Washington (61) and Los Angeles (14). New York state, (87), DC district (61) and California (52) were leading states. 
<br><br>
9. I exported this new sheet to my Drive and opened the Google Sheets version. 
<br><br>
10. The Google sheets I opened automatically suggested to remove white spaces from certain cells in the Amount column, which I allowed. 
<br><br>
11. I froze the top row by going to View<Freeze<1 row. I also made them Bold. 
<br><br>

### ANSWERING THE ASSIGNMENT QUESTIONS <br>

1. __(A) Which industries contributed the most to the Republican and Democratic parties? (B) How much was contributed to each party?__ <br>

* (A) To find which industries contributed most to the two parties, I am going to use PIVOT TABLES. <br>
    * For the ROWS, I chose two: PARTY and INDUSTRY. <br>
    * For the VALUE, I chose INDUSTRY (COUNTA) <br>
    * I copy-pasted the values of each party to separate sheets. <br>
    * After copy-pasting each party’s info to separate sheets, I sorted from Z-A. <br><br>

* The __ANSWERS are:__ <br>
    - Democrats: Total donations were 185, and Media/Entertainment industry made the highest number of donations at 17. <br>
    - Republicans: Total donations made to the party were: 213, and Securities and Investment industry made the highest number of them at 21. <br>
    - Natural Law Party of the United States or 3 got 3 donations, and the highest was made by Oil and Gas at 2. <br><br>
* (B) __How much was contributed to each party?__ For this, another pivot table is required:<br>
    * I went to the AMOUNT column on the datasheet and highlighted it. I then converted it to numbers by selecting the 123 dropdown button and choosing NUMBERS. This removed the $ and also ensured that full values are represented in the pivot table.<br>
    * For the Pivot table, I opened up ROWS as Party and VALUES as AMOUNT. I got the following result:<br>

    * __ANSWER:__ Republicans received the most amount of donations at $30,749,000, followed by the Democrats at $21,553,578. <br><br>

2. __(A) How much did donors from the Misc. Business sector contribute to the Democratic party? (B) Which donors were based in Miami Lakes, FL?__ <br>

    * PIVOT TABLE: ROW: Sector, and VALUE: AMOUNT, SUM <br>

   * Thus, the Misc. Business contributed $10,250,000 or $10.25 million. <br>

    * Now, adding PARTY in COLUMN:<br>

    * Democrats got __$5,425,000 of the total of $10.25 million that Misc Business donated__.
   
![Pivot,'Q2 pivot table'](/two.jpg) <br> 
  <br> 
* B. __Which donors were based in Miami Lakes, FL?__ <br>

    * PIVOT TABLE: ROWS - SECTOR, DONOR, CITY and PARTY <br>
    * __ANSWER__: Cejas, Paul L was based in Miami, FL, and donated to the Democrats <br> <br> 
    * ![Pivot,'Q2 pivot table'](/twobfinal.jpg) <br><br>
3. __(A) What percentage of the tobacco industry’s donations does Philip Morris account for? (B) How much is it?__ <br> <br> 

A. PIVOT TABLE: ROWS - INDUSTRY and DONOR and VALUES - AMOUNT <br>
    * Copy-paste the selected cells to another sheet. <br>
    * To calculate the percentage = (Amount donated by Philip Morris/Total amount donated by Tobacco industry)into 100 <br>
    * In the new sheet, this formula was: =C2/C6 into 100. This resulted in the value: __68.543%__ <br>
    * This equals - $2,070,000 or __$2.07 million.__ <br>

![Pivot,'Q2 pivot table'](/threea.jpg) <br>

4. __(A) Describe (in two to three sentences — no need for a detailed story pitch) one potential story from this dataset that you’d find promising if this were a project you were working on. (B) Give it a headline. (C) Include up to three types of sources you would call to report out the story and a few of the questions you might ask.__<br> <br>
A. Going by the data filtered through the Open Refine too, it is obvious that the tobacco company Philip Morris has been donating regularly to both Republicans and Democrats. It would be interesting to know more about this aspect. <br>
B. Tobacco company Philip Morris donates beyond party lines <br>
C. Three types of sources: <br>
    * Insider sources from the company: I would ask why they found it necessary to contribute to both parties in such large amounts. <br>
    * Quotes from both party representatives: I would ask their relationship with PM, as well as if they plan on any legislation related to the industry.<br>
    * Tobacco industry experts and opponents: Usually these experts have an idea of the legislations and regulations, and I would ask them which ones impact companies like Philip Morris. <br>
    * Health experts - To know more about the impact of tobacco regulations and legislations <br><br>
5. __What data might be suitable to join with this data to provide context or additional stories? Give me two examples.__ <br>
* Data on the legislations and/or regulations related to each industry would help in contextualizing this data. <br>
* Data on donations from previous years too can help in recognizing any trends of donations by various industries/organizations.<br>

