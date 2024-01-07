# FreelancerCDNWebApi

## About the FreelancerCDNWebApi
- Clean Architecture
- ASP.NET Core Web Api
- .NET Core Class Library
- Global Exception Handling
- Curd Operation
- EntityFrameworkCore
- SQL SERVER 2019
- Swagger & SwaggerUI

## Project Architecture details
- a class library with the name *Domain* for our models, Request dto and Response dto

- a class library with the name *Infrastructure* for interfaces such as unit of work 

- a class library with the name *DAL* to communicate with the database

- a class library with the name *IoC* to handle our dependency injections in one layer

- a class library with the name *BL* to implement our business rules 

- a web api .net core to implement our apis

## Develop Domain Layer
> We have 3 tables:
  - *User* is the table that keeps Users data.
  - *Skill* is the table that keeps the Skill types.
  - *UserSkills* is the table that keeps the data that each user has on how many types of Skills.

## Implement Api Layer
we have 5 methods in *UserController* and 1 method in *Skillsontroller*.
> we used 4 types of http requests in these 2 controllers:
  - `[HttpGet]`: use it when the method is going to get data in the output.
  - `[HttpPost]`: use it when the method is going to get some data from input and save it in the database.
  - `[HttpPut]`: use it when the method is going to get some data and update an already saved data.
  - `[HttpDelete]`: use it when the method is going to delete some data from the database.
