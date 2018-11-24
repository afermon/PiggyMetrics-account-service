# Piggy Metrics (Kubernetes) - Account service

[![CircleCI](https://circleci.com/gh/afermon/PiggyMetrics-account-service.svg?style=svg)](https://circleci.com/gh/afermon/PiggyMetrics-account-service) [![codecov](https://codecov.io/gh/afermon/PiggyMetrics-account-service/branch/master/graph/badge.svg)](https://codecov.io/gh/afermon/PiggyMetrics-account-service) [![GitHub license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/afermon/PiggyMetrics-account-service/blob/master/LICENCE)

Contains general user input logic and validation: incomes/expenses items, savings and account settings.

Method	| Path	| Description	| User authenticated	| Available from UI
------------- | ------------------------- | ------------- |:-------------:|:----------------:|
GET	| /accounts/{account}	| Get specified account data	|  | 	
GET	| /accounts/current	| Get current account data	| × | ×
GET	| /accounts/demo	| Get demo account data (pre-filled incomes/expenses items, etc)	|   | 	×
PUT	| /accounts/current	| Save current account data	| × | ×
POST	| /accounts/	| Register new account	|   | ×

For more information please refer to the main repository [afermon/PiggyMetrics-Kubernetes](https://github.com/afermon/PiggyMetrics-Kubernetes)

## Credits

* Forked from [sqshq/PiggyMetrics](https://github.com/sqshq/PiggyMetrics)