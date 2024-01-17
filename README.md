
# Stackoverflow_survey_2023_insights


StackOverflow conductes its annual survey, drawing responses from over 90000 developers worldwide. This expansive dataset provides a comprehensive look into the evolving landscape of the developer community, shedding light on learning patterns, technology preferences, and emerging trends.
as for practice and getting insights that answers my own question related to programming languages, databases, etc that are been used and desired by developers globally to be used in future.

###### the shape of the dataset is (89184, 84)
![image](https://github.com/nmrata0612/Stackoverflow_survey_2023_insights/assets/143874811/9918ec23-efb1-4ae0-bf08-5408313e21f2)



![image](https://github.com/nmrata0612/Stackoverflow_survey_2023_insights/assets/143874811/319c547b-63dc-4029-8a48-3a28878bf35c)

the MainBranch column states if the developer is a professional coder, a student, persue coding as an hobby or was a former coder (either retired or switched the field)

the dataset contain rows that are filled with irrelavent Data
![image](https://github.com/nmrata0612/Stackoverflow_survey_2023_insights/assets/143874811/b3b636a3-61f9-4187-9b52-4c9a8317ed36)

removed the unwanted data.
![image](https://github.com/nmrata0612/Stackoverflow_survey_2023_insights/assets/143874811/8a925037-4569-48a0-8ebc-49f1f7c5ca5c)


the Employment column contain multiple values.
![image](https://github.com/nmrata0612/Stackoverflow_survey_2023_insights/assets/143874811/522324c8-5807-4f98-ad39-a1d08107bc45)
these values state that people who are independent contractors are also part time student, but primarily is a independent contractor.
first value as the being the primary Employment status.
![image](https://github.com/nmrata0612/Stackoverflow_survey_2023_insights/assets/143874811/ccf458bf-d05c-4edb-91ec-fa29c6b5066d)

And handled the null values as 'prefer not to say'.

the YearsCode column defines the number of years a person has done coding
the data type was object and contained values such as less than 1 year, more than 50 years and I prefer not to say.
![image](https://github.com/nmrata0612/Stackoverflow_survey_2023_insights/assets/143874811/3cf88967-fed3-4b2d-b6f7-8041390e3be8)
the values 'less than 1 year' and 'more than 50 years' was converted to 0 and 50.
changes the data type and handled the missing values as finding the mean based on the employment type and filled the values.
eg. ![image](https://github.com/nmrata0612/Stackoverflow_survey_2023_insights/assets/143874811/c824287f-2ee9-428c-afd7-7f07283f3dfb)

Extracted the columns from the df into a new DataFrame named 'required_data', that i will be considering for further process.
![image](https://github.com/nmrata0612/Stackoverflow_survey_2023_insights/assets/143874811/1f34c338-0826-4d38-a811-64ac7717eb06)


to find some information about the languages, cleaned the data and made it into a proper format.

![image](https://github.com/nmrata0612/Stackoverflow_survey_2023_insights/assets/143874811/60c8d0b6-e2d5-45b3-9577-a0a0251bafa0)

made a seperate DataFrame to store the LanguagesHaveWorkedWith column.
we need to explode the data to find the count of different languages 
![image](https://github.com/nmrata0612/Stackoverflow_survey_2023_insights/assets/143874811/2f3561a5-ef29-4fea-91be-31a09cbe9ba9)
we can merge the LanguageWorkedWithDf with required_data to find the answers to scenario based conditions like:
![image](https://github.com/nmrata0612/Stackoverflow_survey_2023_insights/assets/143874811/6c863006-e8db-4c4c-a247-fe05b44e35e0)
this shows top 10 languages used by professional

![image](https://github.com/nmrata0612/Stackoverflow_survey_2023_insights/assets/143874811/d14bdfcc-b48a-4af2-8ffa-11c55a0e5d05)
top 10 languages used for data or business analysis.

In column LanguageWantToWorkWith contain list of languages developer either want to continue or want learn new languages.
To identify the new languages other than the that is being used currently, I created a new column name 'continueLang' and 'newLang', to find the increasing use of language in future
![image](https://github.com/nmrata0612/Stackoverflow_survey_2023_insights/assets/143874811/75892641-4a21-471c-8876-64a038267cd9)

it can be seen that the most desired language desired by developers is Rust
![image](https://github.com/nmrata0612/Stackoverflow_survey_2023_insights/assets/143874811/b173f551-c5b1-4fdd-8aa8-cefc6a8ccc81)

#### performed same operations with databases, and other columns.
## Demo

Insert gif or link to demo

[pdf file of the Dashboard](https://github.com/nmrata0612/Stackoverflow_survey_2023_insights/blob/main/Dashboard.pdf)

![image](https://github.com/nmrata0612/Stackoverflow_survey_2023_insights/assets/143874811/bede798b-39b3-4cdb-9955-25aa7b00e3e1)

[link to the power bi Dashboard](https://github.com/nmrata0612/Stackoverflow_survey_2023_insights/blob/main/Dashboard.pbix)

[Stack Overflow Annual Developer Survey](https://insights.stackoverflow.com/survey)
