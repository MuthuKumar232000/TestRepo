# ct-load-test

## Introduction

This project built exposes the load testing of  Crosstower APIs on JMeter

### Technology Considerations
    1. Programming Language                Java
    2. Version                             apache-jmeter-5.4.1
    3. Build Tool                           JMeter
    
## Introduction to JMeter
 - Apache JMeter is a testing tool used for analyzing and measuring the performance of different software services and products. It is a pure Java open source software used for testing Web Application or FTP application.
It is used to execute performance testing, load testing and functional testing of web applications. JMeter can also simulate a heavy load on a server by creating tons of virtual concurrent users to the web server.

## How does JMeter perform Testing?
 - Let’s have a look at the different steps performed by JMeter during testing:
	1.It creates a request and sends to the server.
	2.It receives the response from servers, collects them and visualizes those details in a chart or graph.
	3.It processes the response from the server.
	4.It generates the test result in several formats such as text, XML, JSON so that the tester can analyze data.
 - Now that you know what is JMeter and how it works, let’s move on and have a look at the prerequisites for installing JMeter.
 - Then, you can create your own test plan in JMeter with the help of different elements.

## Install JMeter
 - The Operating Systems compatible with JMeter are:
	Linux
	Windows
	Mac OS
	Ubuntu
 - Download the Jmeter from https://jmeter.apache.org/download_jmeter.cgi
 - Once Download the Jmeter files on Systems compatible then simply unzip the zip/tar file into the directory where you want JMeter to be installed. There is no tedious installation screen to deal with.

## Core Logic Implementation
### Crosstwer Script and Test-Data
 - We created  4 script on Jmeter
 	|Scrpit|
	|:-----------:|
	|[001_Script](https://github.com/MuthuKumar232000/TestRepo/blob/master/README.md#001_script)
	[002_Script](https://github.com/MuthuKumar232000/TestRepo/blob/master/README.md#002_script) 
	[003_Script](https://github.com/MuthuKumar232000/TestRepo/blob/master/README.md#003_script) 
	[004_Script](https://github.com/MuthuKumar232000/TestRepo/blob/master/README.md#004_script)|
 - We created 6 csv test-data files
 	|Test-Data|
	|:---------:|
	|[001_Script_UserEmail](https://github.com/MuthuKumar232000/TestRepo/blob/master/README.md#001_script_useremail) 
	[001_Script_UserToken](https://github.com/MuthuKumar232000/TestRepo/blob/master/README.md#001_Script_UserToken) 
	[001_Script_Curreny_Details](https://github.com/MuthuKumar232000/TestRepo/blob/master/README.md#001_Script_Curreny_Details) 
	[001_Script_Coin](https://github.com/MuthuKumar232000/TestRepo/blob/master/README.md#001_Script_Coin) 
	[001_Script_bucket](https://github.com/MuthuKumar232000/TestRepo/blob/master/README.md#001_Script_bucket) 
	[001_Script_bucketid](https://github.com/MuthuKumar232000/TestRepo/blob/master/README.md#001_Script_bucketid)|

## 001_Script
  |Request|Endpoint|Functionality|
 |:-----:|:------:|:-----------:|
 |GET   |/api/ticker/list | Ticker Data|
 |GET   |/api/user  | User Info|
 |GET    |/api/user/portfolio | User portfolio| 
 |GET    |/api/order/create-order  | Order Symbols List | 
 |GET |/api/order/symbols/fee | Crypto Trading Fee with Symbol | 
 |POST   |/api/order/preview-order | Preview Order |
 |GET   |/api/order/history | User Order History |
 |GET   |/api/withdraw/inr/fee  | Inr Withdraw Fee |
 |GET    |/api/withdraw/crypto/fee | Crypto Withdraw Fee| 
 |GET    |/api/inr/payment-gateway  | Inr Payment Gatway List | 
 |GET |/api/inr/deposit | Inr Deposit | 
 |GET   |/api/crypto/deposit-address | Crypto Depost address with Curreny Id |
 |GET    |/api/deposit-withdraw-history | User Deposit Withdraw History | 
 |GET    |/api/inr/deposit/track-payment  | Track UPI Deposit | 
 |GET |/api/gift/list | List Gift Code | 
 |GET   |/api/order-bucket/default | List Default Baskets |
 |GET  |/api/order-bucket | List User Baskets |
 |GET   |/api/order-bucket/size | Basket Configuration |
 |GET   |/api/order-bucket/history | List Basket Order History| 
 |GET   |/api/order-bucket/currency   | Basket currency Info | 

## 002_Script
  |Request|Endpoint|Functionality|
 |:-----:|:------:|:-----------:|
 |POST   |/api/user-check | User check|
 |POST   |/api/auth/register  | User Registration|
 |POST   |/api/bank/add | Bank Add| 
 |POST   |/api/kyc/add  | Kyc Add| 
 |POST |/api/order/symbols/list | Create Tokenl | 
 |POST   |/api/order-bucket | Create Basket |
 |PUT   |/api/order-bucket | Update Basket |

## 003_Script
|Request|Endpoint|Functionality|
 |:-----:|:------:|:-----------:|
 |POST   |/api/user-check | User check|
 |GET   |/api/user  | User Info|
 |GET    |/api/user/portfolio | User portfolio| 
 |GET    |/api/order/create-order  | Order Symbols List | 

## 004_Script
|Request|Endpoint|Functionality|
 |:-----:|:------:|:-----------:|
 |POST   |/api/order/symbols/list | Create Order|
 |POST   |/api/verification/otp  | Otp On Register Phone Number|
 |POST    |/api/withdraw/inr | Withdraw Inr| 
 |POST    |/api/withdraw/crypto | Crypto Withdraw | 
 |POST   |/api/inr/deposit/initiate-payment  | Initiate UPI Deposit|
 |POST   |/api/gift/create | Create Gift Code| 
 |POST   |/api/gift/redeem  | Redeem Gift Code | 

## 001_Script_UserEmail
|Variable|
 |:-----:|
 |Email, Phone number, APIKey, ScreatKey, Bank number, Pan Number |

## 001_Script_UserToken
|Variable|
 |:-----:|
 |Email APIKey |

## 001_Script_Curreny_Details
|Variable|
 |:-----:|
| Base Curreny Id, Base Curreny Name, Quote Curreny Id, Quote Curreny Name, Curreny side(BUY,SELL,CONVERT), Quantity |

## 001_Script_Coin
|Variable|
 |:-----:|
| Coin name|

## 001_Script_bucket
|Variable|
 |:-----:|
| Bueket name |

## 001_Script_bucketid
|Variable|
 |:-----:|
| Bueket name, Bueket Id |

## Sample User file
|Files|
 |:-----:|
| 001_Script_crosstests100 (100Users), 001_Script_crosstestsh5000 (100Users), 001_Script_crosstestsm10000 (100Users), 001_Script_crosstestst1000 (100Users) |

### Build steps
 - Download all Script, Test-data and Report folders and stored in any directory
 - After Instell Jmeter, If you are using Windows, just run the file ```/bin/jmeter.bat``` to start JMeter in GUI mode 
 - Once open JMeter GUI Tool import the given script files by ``` File->Open->Select the Script file->Open ```
 - After open the Script, we have to import the stored directory path  on directory (User Define Variable Config Element) for access Test-Data files
 - Before We Run to Script, We have clear the ```001_Script_UserToken and 001_Script_bucketid``` Test-data on directory
 - The ``` Dynamic User Email Data is Given by 001_Script_UserEmail file```and ``` Dynamic bucket name is Given by 001_Script_bucket```->enter concurrent user details 001_Script_UserEmail and run the Script
 - ```001_Script_Curreny_Details and  001_Script_Coin ```have default values of have coins details, base and quote currency details

### Summary Report 
 - The Load result will get by Using different Listener ``` (View Results Tree, View Results in Table and Summary Report)```

