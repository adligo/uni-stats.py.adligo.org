# Labor Force Statistics from the Current Population Survey

- [Webpage](https://www.bls.gov/cps/tables.htm#weekearn)
- [Initial Data File Url](https://www.bls.gov/cps/data/aa2025/cpsa2025.xlsx)
- [Initial Data File](12/cpsa2025.xlsx)


Notes 

Created [laborForce2025.ods](12/laborForce2025.ods) by copying data from the initial data file and renaming these columns, and formatting as a csv file.

##### Year 

  From column A

##### Total_Population

  From column B in thousands / Civilian noninstitutional population
  
##### Labor_Force_Population

  From column C in thousands / Civilian labor force / Total
  
##### Labor_Force_Pct 

  From column D / Civilian labor force / Percent of population

##### Employed_Pct

  From column F / Civilian labor force / Employed

##### Unemployed_Population

  From column I / Civilian labor force / Unemployed / Number

##### Unemployed_Pct

  From column J / Civilian labor force / Unemployed / Percent of labor force

##### Other_Population

  From column K / Not in labor force

##### Check

  Added Other_Population to Labor_Force_Population

##### Diff

  Compared the Check Column to Total_Population

