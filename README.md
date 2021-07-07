# Shop Management Mule 4 API

## Overview

The following repo contains shop-management-mule4 application

Should be used only for educational purpose

## How to deploy applicaton

for building jar file run from cmd:

$ mvn clean install -Dmule.env=dev -Druntime.key=******

after this commend, the .jar file is build in target folder

for deploying on CloudHub run from cmd:

$ mvn clean install deploy -DskipTests -Dmule.env=dev -Druntime.key=******

## How to test application

for running tests, run from cmd the followint command:

$ mvn test -Dmule.env=dev -Druntime.key=******
 