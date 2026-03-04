# Statistics about the US University System

One of the challenges about getting statistics on college and higher education it's simply the complexity of the data.  It is surveyed by various government institutions at various times and provided in various formats, generally in non-normal forms.  This project attempts to simplify some of that information by taking it in various raw formats, massaging it into normal forms, and then calculating statistics on the normal data. 

# Notes

In short, Numbers may never lie, but they often disagree.

One of the first challenges you'll notice if you really take a look at this data is that sometimes data is split out in various ways that are hard to reassemble simply.  For example when you compare Citations 3 and 4, they both show average weekly earnings; however in Citation 4 people with bachelor's degrees and higher are lumped together while in citation number three, these are split out into separate values.  This creates a secondary statistical problem you have to solve first, which is to determine the correlation from years 2000 to 2021 of people with just bachelor's degrees and people with bachelor's degrees and higher to the data in citation 4.  If you want to see the data for people with just 4 year bachelors degrees.

In order to offset for this difference we added the following columns to weeklyWages2000-2021.ods. 

 - B & H  The sum of the Bachelor's degree and Advanced degree divided by 2
 - B % The percentage of the Bachelor's degree over the value from the new B & H column
 - Average The average of all of the B % rows which turned out to be 88.5%

- [weeklyWages2000-2021.ods](raw-data/weeklyWages2000-2021.ods)

- [bls.gov survey comments](etc/BLS_SURVEY_COMMENTS.md)

# Citations

### Citation # 1 

- [How much does college cost 2012-2022?](https://nces.ed.gov/fastfacts/display.asp?id=76#:~:text=$4%2C000%20for%20public%20institutions%2C%20which)
- [How much does college cost 2012-2022? (Saved as a PDF)](raw-data/Citation#1_FastFacts_TuitionCostsOfCollegesAndUniversities)

##### Figure 2. Average tuition and fees of degree-granting institutions for first-time, full-time degree/certificate-seeking undergraduate students, by level and control of institution: Academic years 2012–13 through 2022–23

- [collegeCosts2012-2022.csv in UTF-8](raw-data/collegeCosts2012-2022.csv)
- [collegeCosts2012-2022.ods](raw-data/collegeCosts2012-2022.ods)

### Citation # 2

- [Who was employed 2013-2023?](https://nces.ed.gov/programs/coe/indicator/cbc)
- [Who was employed 2013-2023? (Saved as a PDF)](raw-data/Citation#2_WhoWasEmployed.pdf)

Note Figures 2 and 4 don't really add up, as not employed != unemployed.

##### Figure 2. Employment rates of 25- to 34-year-olds, by educational attainment: 2013 through 2023

- [whoWasEmployed2013-2023.csv in UTF-8](raw-data/whoWasEmployed2013-2023.csv)
- [whoWasEmployed2013-2023.ods](raw-data/whoWasEmployed2013-2023.ods)

##### Figure 4. Unemployment rates of 25- to 34-year-olds, by educational attainment: 2013 through 2023

- [unemployed2013-2023.csv in UTF-8](raw-data/unemployed2013-2023.csv)
- [unemployed2013-2023.ods](raw-data/unemployed2013-2023.ods)

### Citation # 3

- [What did they make 2000 - 2021?](https://usafacts.org/articles/is-college-worth-it-the-price-of-college-is-rising-faster-than-wages-for-people-with-degrees/)
- [What did they make 2000 - 2021? (Saved as a PDF)](raw-data/Citation#3_ThePriceOfCollegeIsRisingFasterThanWagesForPeopleWithDegrees_USAFacts.pdf)

##### Wages for people with bachelor’s degrees have risen 5% since 2000, compared to 0.1% for people with some college or an associate degree.

- [weeklyWages2000-2021.csv in UTF-8](raw-data/weeklyWages2000-2021.csv)
- [weeklyWages2000-2021.ods](raw-data/weeklyWages2000-2021.ods)

### Citation # 4

- [What did they make 2000 - 2024?](https://www.bls.gov/opub/ted/2025/median-weekly-earnings-by-educational-attainment-first-quarter-2025.htm)
- [What did they make 2000 - 2024? (Saved as a PDF)](Citation#4MedianWeeklyEarningsByEducationalAttainmentFirstQuarter2025_TheEconomicsDaily_U.S.BureauOfLaborStatistics.pdf)

##### Median usual weekly earnings of full-time wage and salary workers age 25 years and over, by educational attainment, quarterly averages, not seasonally adjusted

- [weeklyWagesByQuarter2000-2024.csv in UTF-8](raw-data/weeklyWagesByQuarter2000-2024.csv)
- [weeklyWagesByQuarter2000-2024.ods](raw-data/weeklyWagesByQuarter2000-2024.ods)

### Citation 5

 - [Cost of College 1963-2025](https://educationdata.org/average-cost-of-college-by-year)
 - [Cost of College 1963-2025 (Saved as a PDF)](raw-data/Citation#5CostOfCollege1963-2025.pdf)
 
##### Annual Cost of College Tuition & Fees

- [collegeCosts1963-2022.csv  in UTF-8](raw-data/collegeCosts1963-2022.csv)
- [collegeCosts1963-2022.ods](raw-data/collegeCosts1963-2022.ods)

### Citation 6

- [Per Student Debt 2007-2025](https://educationdata.org/average-student-loan-debt-by-year)
- [Per Student Debt 2007-2025 (Saved as a PDF)](https://educationdata.org/average-student-loan-debt-by-year)

##### Average Student Loan Debt by Year

- [perStudentDebt2007-2025.csv in UTF-8](raw-data/perStudentDebt2007-2025.csv)
- [perStudentDebt2007-2025.ods](raw-data/perStudentDebt2007-2025.ods)

### Citation 7

https://ticas.org/wp-content/uploads/2023/12/Quick-Facts-About-Student-Loan-Debt-2023.pdf

Figure 2: Share of Completers with Student Loan Debt Over Time  

### Citation 8 

Citation#8CollegeEnrollmentAndWorkActivityfOfHighSchoolGraduatesNewsRelease-2024A01Results.pdf


https://www.bls.gov/news.release/hsgec.htm


### Citation 9

https://www.lisep.org/tru
https://cdn.prod.website-files.com/63ba0d84fe573c7513595d6e/699754c2a140ad45e4e4e124_TRU%20%26%20TWE%20Data%20January%202026.xlsx

Note this is the whole population not just 25-33 year olds, like Figure 2 Citation 2.

Renamed columns from raw-data/699754c2a140ad45e4e4e124_TRU%20%26%20TWE%20Data%20January%202026.xlsx to
lisepUnemploymentMothly1995-2025.ods

No High School from LISEP True Rate of Unemployment Out of the Population - No High School
High School Degree from LISEP True Rate of Unemployment Out of the Population - High School Degree or Equivalent
Some College from LISEP True Rate of Unemployment Out of the Population - Some College
Bachelor's Degree from LISEP True Rate of Unemployment Out of the Population - Bachelor's Degree
Advanced Degree from LISEP True Rate of Unemployment Out of the Population - Advanced Degree


[699754c2a140ad45e4e4e124_TRU&TWEDataJanuary2026.ods](699754c2a140ad45e4e4e124_TRU&TWEDataJanuary2026.ods)


### Citation 10 

Direct Python-UNO Bridge
- [Webpage](https://www.openoffice.org/udk/python/python-bridge.html)
- [Other Details](citation-details/Citation#10_details.md)

### Citation 11

- [Webpage](https://catalog.data.gov/dataset/labor-force-participation-rate-us-and-california)
- [Raw UTF-8 CSV File](raw-data/labor_force_participation_rate__us_and_california.csv)
- [Other Details](citation-details/Citation#11_details.md)

### Citation 12

- [Webpage](https://www.bls.gov/cps/tables.htm#weekearn)
- [Raw UTF-8 CSV File](raw-data/laborForce2025.csv)
- [Other Details](citation-details/Citation#12_details.md)

### Citation 13

https://nces.ed.gov/programs/digest/current_tables.asp

Click current or 2025
Chapter 5.  Outcomes of Education.
Table 501.50
  Why is 2023 the most recent year with data?
  
  
### Citation 14

https://www.bls.gov/cps/definitions.htm#:~:text=People%20waiting%20to%20start%20a,receipt%20of%2C%20unemployment%20insurance%20benefits.

