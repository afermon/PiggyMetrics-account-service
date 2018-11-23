[![CircleCI](https://circleci.com/gh/afermon/PiggyMetrics-account-service.svg?style=svg)](https://circleci.com/gh/afermon/PiggyMetrics-account-service)
[![codecov](https://codecov.io/gh/afermon/PiggyMetrics-account-service/branch/master/graph/badge.svg)](https://codecov.io/gh/afermon/PiggyMetrics-account-service)
[![GitHub license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/sqshq/PiggyMetrics/blob/master/LICENCE)

# PiggyMetrics

**A simple way to deal with personal finances**

This is a proof-of-concept application, which demonstrates [Microservice Architecture Pattern](http://martinfowler.com/microservices/) using Spring Boot, Spring Cloud, Docker, Kubernetes and Google Cloud Plataform. With a pretty neat user interface, by the way.

**For more information please refer to the [Parent project](https://github.com/afermon/PiggyMetrics)**

## Functional services

PiggyMetrics was decomposed into three core microservices. All of them are independently deployable applications, organized around certain business domains.

<img width="880" alt="Functional services" src="https://cloud.githubusercontent.com/assets/6069066/13900465/730f2922-ee20-11e5-8df0-e7b51c668847.png">

#### Account service
Contains general user input logic and validation: incomes/expenses items, savings and account settings.

Method	| Path	| Description	| User authenticated	| Available from UI
------------- | ------------------------- | ------------- |:-------------:|:----------------:|
GET	| /accounts/{account}	| Get specified account data	|  | 	
GET	| /accounts/current	| Get current account data	| × | ×
GET	| /accounts/demo	| Get demo account data (pre-filled incomes/expenses items, etc)	|   | 	×
PUT	| /accounts/current	| Save current account data	| × | ×
POST	| /accounts/	| Register new account	|   | ×

## Refereces
* Forked from [sqshq/PiggyMetrics](https://github.com/sqshq/PiggyMetrics)