# Shop Management Mule 4 API

## Overview

The following repo contains shop-management-mule4 application

Should be used only for educational purpose

## How to deploy applicaton

clone this application by command:

**git clone https://github.com/marianburdianov/shop-management-mule4.git**

change directory to cloned repository

for building jar file run from cmd:

**$ mvn clean install -Dmule.env=dev -Druntime.key=****** **

after this commend, the .jar file is build in target folder

for deploying on CloudHub run from cmd:

**$ mvn clean package deploy -DskipTests -Dusername=marianburdianov1 -Dpassword=******** -Denviroment=Sandbox -Dmule.version=4.3.0 -Dworker=1 -Dworker.type=Micro -Dapplication.name=shop-management-mule4 -DmuleDeploy
  **

## How to test application

for running tests, run from cmd the followint command:

**$ mvn test -Dmule.env=dev -Druntime.key=******  **
 