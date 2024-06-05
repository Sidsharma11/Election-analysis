# Election Analysis
Live Report link:

## Project Overview
C-Voter is a private media company and they wanted to telecast a show on Lok
Sabha elections 2024 in India. Unlike other channels they do not want to have a
debate on who is going towin this election, they rather wanted to present insights
from 2014 and 2019 elections without any bias and discuss less explored themes
like voter turnout percentage in India. As a data analyst in the company, the task 
is to  generate meaningful insights from data. 

## Dataset Understanding
The dataset consist of 3 csv fies.

## Steps Performed

### Step 1: Date Cleaning:
1): Peformed task such as appending the two tables,Clean,trim,replace values etc.

![Screenshot 2024-06-03 135320](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/a3779d7f-5197-4df1-83b4-b355ff881f9a)

2): Replaced values --In 2014, Andhra Pradesh underwent bifurcation. For simplicity, all constituencies
from thatyear should be attributed to Telangana state. This includes constituencies
such as Adilabad, Hyderabad, Warangal, etc., which should be considered part of
Telangana rather than Andhra Pradesh for the year 2014.


![Screenshot 2024-06-03 231706](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/2f3a9ba7-2a95-4c0b-9620-68cbb9a1edc0)


### Step 2 : Crafted SQL queries to address the specified business questions given below:

#### Q-1) List top 5/ bottom 5 constituencies of 2014 and 2019 in terms of voter turnout ratio?

![Screenshot 2024-06-05 223907](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/2ff0f6b3-b0d2-4c5f-b9ac-4b813d00999d)

####            Top 5 Constituency in terms of voting percentage in the year 2014
![Screenshot 2024-06-05 223952](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/72bdaa63-ab64-47de-9172-b20241668a92)

####            Bottom 5 Constituency in terms of voting percentage in the year 2014
![Screenshot 2024-06-05 224512](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/012f4e7a-f000-4dc4-a28d-70e8625db2d9)

####            Top 5 Constituency in terms of voting percentage in the year 2019
![Screenshot 2024-06-05 224621](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/f048b1e0-9c41-4cca-af3b-4dd988f05ae0)

####            Bottom 5 Constituency in terms of voting percentage in the year 2019
![Screenshot 2024-06-05 224738](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/d083ebe7-a345-4048-9daf-83c0d9c50310)


#### Q-2) Listtop 5/ bottom 5 states of 2014 and 2019 in terms of voter turnout ratio?

![Screenshot 2024-06-05 225005](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/55ed3323-e7ce-4ed8-8890-09ee7e961ce6)

####     Top 5 States in terms of voting percentage in the year 2014
![Screenshot 2024-06-05 225033](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/3ca4ef72-9b85-4036-951f-77a42a7ab501)

####     Top 5 States in terms of voting percentage in the year 2019
![Screenshot 2024-06-05 225045](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/bcf7be12-5f9c-4f2b-a519-2948292188eb)

####     Bottom 5 States in terms of voting percentage in the year 2014
![Screenshot 2024-06-05 225054](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/1d4610a7-f44d-4b07-8b47-bc9271b12c3e)

####     Bottom 5 States in terms of voting percentage in the year 2019
![Screenshot 2024-06-05 225116](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/f847e1cf-defd-4ab0-a15e-41f2e9bebaff)

#### Q-3) Which constituencies have elected the same party for two consecutive elections,rank them by % of votes to that winning party in 2019?

![Screenshot 2024-06-05 234123](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/626e56f0-5d96-4178-8b36-031f540e9939)
![Screenshot 2024-06-05 234137](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/bb25bcdc-be29-4b50-be8c-b050c3c22056)

![Screenshot 2024-06-05 234603](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/7fe7f579-0522-408a-bee2-5764b2e1e01c)
![Screenshot 2024-06-05 234623](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/d08f5dbf-81c5-4213-ba19-fd3ec4b931a5)
![Screenshot 2024-06-05 234651](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/ebd886cc-40c3-43b0-9af6-5b5cd0cceddd)

#### Q-4)Which constituencies have voted for different parties in two elections (list top 10 based on difference (2019-2014) in winner vote percentage in two elections)

Created view 'winner_2014'and 'winner_2019' using
![image](https://github.com/Sidsharma11/Election-analysis/assets/167175484/737e0595-cbf6-4337-805c-e4a9438ee040)

used view 'winner_2014' and 'winner_2019'
![Screenshot 2024-06-05 235251](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/1a1969fe-0acf-4b59-8175-259b091090f7)
![Screenshot 2024-06-05 235321](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/c5dc45be-ca14-4364-b2ad-99fc924876c0)

#### Q-5)Top 5 candidates based on margin difference with runners in 2014 and 2019.

created temporary tables 'winner' and runner_up
![Screenshot 2024-06-06 004709 - Copy](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/78f01964-580d-452f-af22-ca5451103e0b)

![Screenshot 2024-06-06 004740](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/aad4796b-6280-4917-9590-336af090668b)
![Screenshot 2024-06-06 004803 - Copy](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/4d9a17c7-4297-4293-997b-66220eee1ace)
![Screenshot 2024-06-06 004819 - Copy](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/ec572256-8cd0-4b24-b5bc-38f74acf409d)
![Screenshot 2024-06-06 004841](https://github.com/Sidsharma11/Atliq_sales_report/assets/167175484/43b6c0b6-7d94-491e-b7ff-019b7058a99a)








