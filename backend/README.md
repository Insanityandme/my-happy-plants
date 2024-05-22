<div align="center">

# MyHappyPlants Backend
[Install](#install) • [Testing](#testing) • [Contact](#contact)

--- 

<img src="https://github.com/Insanityandme/my-happy-plants/assets/1380257/e976f1b8-922e-49ce-9d8e-450c451496e0"/>

</div>

---
### Table of Contents
- [Introduction](#introduction)
- [Installation](#install)
- [Testing](#testing)
- [Contact](#contact)

# Introduction
MyHappyPlants was originally an incomplete student project written in Java, using JavaFX for all GUI related code. 

It was a Java desktop application that exists to help you organize and keep track of your plants at home.
Using Trefles extensive API to get detailed information about your species of plants. 

We decided to start over from scratch and turn it into a Java based backend API using Javalin, a lightweight web framework for Java and Kotlin.

Our frontend is written in Javascript using React and is located here: https://github.com/Insanityandme/systemutv-II-frontend

# Install
Our application is divided into two seperate parts
+ backend
+ frontend

## Back-end
### Initial Setup
1. ```git clone https://github.com/Insanityandme/systemutv-II-backend.git```

### Instructions for environment variables
1. We use environment variables in development for our secret KEYS
2. In your operating system be it Windows, Linux or Mac, set the environment variable `TREFLE_API_KEY` to your Trefle API key

Instructions for MACOSX: https://phoenixnap.com/kb/set-environment-variable-mac

Instructions for WINDOWS: https://phoenixnap.com/kb/windows-set-environment-variable

### Instructions for databases and uploads
1. We are using SQLite for our simple database
2. Create or copy two database files  ```myHappyPlantsDB.db``` and ```myHappyPlantsDBTEST.db```
3. Create a folder named ```resources``` in src/main and put them in there
4. Create an empty folder named ```uploads``` in the same directory

## Using IntelliJ
1. If you are using an IDE such as IntelliJ and Eclipse you need to install the Maven plugin for your environment if it isn't already installed. (It's most likely already installed)
2. Navigate to the file Javalin.java in src/main/java/se/myhappyplants/javalin/
3. Run Javalin.java and now the server should be running!

## Using terminal
1. Make sure you have maven installed on your computer (SEE: https://www.baeldung.com/install-maven-on-windows-linux-mac)
2. run ```mvn install``` in the root of the project
3. run ```mvn compile``` in the root of the project
4. run ```mvn clean package``` in the root of the project
5. run ```java -jar .\target\MyHappyPlants-1.0-SNAPSHOT-jar-with-dependencies.jar```
6. The server should now be running!


## Front-end
You can find instructions for the frontend here: https://github.com/Insanityandme/systemutv-II-frontend

# Testing 

## Using IntelliJ
1. Go into src/main/testing folder
2. If Mockito and Junit is installed (it usually is included in your IDE or will be installed through Maven)
3. Run all files except Helper.java
4. Done

## Using terminal
1. Same as with running the server you need to have Maven installed globally on your computer for this to work properly
1. cd into root of the project
2. if you've run ```mvn install``` and ```mvn clean package``` you are good to go.
3. run ```mvn clean test```
4. Done

# Contact
You are welcome to contact me at bengtegardbook@gmail.com if you have any questions on how to setup this environment.
There might be some mistakes in our installation guide and I apologize for that if that's the case.
