
# Project Title: Performance Testing of COVID-19 Global Statistics API

## Project Summary : 
This project focuses on performance testing of the COVID-19 Global Statistics API from disease.sh (Server:https://disease.sh/v3/covid-19/all) through load and stress testing. The tests simulate 120,000 users over 12 hours and identify the system's bottleneck point and capacity TPS through stress test .The objective is to evaluate the API's response time, stability, and reliability under various load conditions. The tests are designed to simulate multiple scenarios, such as high traffic and sustained usage, to ensure the API can handle real-world demands.

## Prerequisites
- Java (Latest version)
- Apache JMeter (Latest version)

## How to Run Performance Tests?
### Run Test Plan and Generate Report
###Execute the following commands:
- ```Run the jmeter.bat (Windows) or jmeter.sh (Unix) script from the bin directory. ```
- ```Open JMeter GUI and load the provided test plan file (covid19_test_plan.jmx).```
- ```Open JMeter GUI and load the provided test plan file (covid19_test_plan.jmx).```
- ```Click the green Start button in JMeter to begin the test.``` 
- ```View results using the added listeners (e.g., View Results Tree, Summary Report).``` or

## Using JMeter CLI
###Execute the following command to run the test plan in non-GUI mode:

- ```
  To Run Test Plan: Execute: jmeter -n -t yourFile.jmx -l yourFile.csv.```
- ```
  To Generate Report: Execute:jmeter -n -t yourFile.jmx -l yourFile.csv -e -o Reports.```

## Resources:

## Load Test and Stress Test reports in Excel format.
You can download the Excel files from the following links:
- [Load&stresstest.xlsx](https://docs.google.com/spreadsheets/d/1NQoul8f9fX15vutBTHN46yBVwDtDyF7A/edit?usp=sharing&ouid=106900521374584856661&rtpof=true&sd=true)

## Screetshot of Excel sheets:

## Load Test:

![Load](https://github.com/ShuhanaRiya09/Random-Covid-19-API-Performance-Test/assets/108625095/2e171cf0-e342-4fcc-bda0-6c8d3fa314c2)
## Stress Test:

![s](https://github.com/ShuhanaRiya09/Random-Covid-19-API-Performance-Test/assets/108625095/c5903eb9-7c26-42a1-baf4-d2cb342af1db)

## Outputs:

## Jmeter HTML Report:

![1report](https://github.com/ShuhanaRiya09/Covid-19-API-Performance-Test/assets/108625095/ea72a44c-fd7f-4fb4-ab9a-4098e56babbb)


## Bottleneck and Capacity TPS :

## Bottleneck Point -
The system starts to show a 0.67% error rate at a TPS of 9.15

## Capacity TPS -
The maximum sustainable TPS the system can handle without errors is 7.52

## Conclusion :
The performance testing of the Random User API demonstrated its ability to handle the expected load of 120,000 users over 12 hours. The Load Test confirmed the API meets the required TPS, while the Stress Test identified the bottleneck at which a 1% error rate occurs. These insights provide a foundation for future optimizations and scaling efforts, ensuring the API remains robust under increased loads.



