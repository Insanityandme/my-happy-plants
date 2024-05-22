<div align="center">

# MyHappyPlants
[Introduction](#introduction) • [Install](#install) • [Testing](#testing) • [Contact](#contact)

--- 
<img src="https://github.com/Insanityandme/my-happy-plants/assets/1380257/3f345eca-fbae-458a-8dc8-6db6727b023d"/> 

</div>

---

# Introduction
MyHappyPlants was originally an incomplete student project written in Java, using JavaFX for all GUI related code. 

It was a Java desktop application that exists to help you organize and keep track of your plants at home.
Using Trefles extensive API to get detailed information about your species of plants. 

We decided to start over from scratch and turn it into a Java based backend API using Javalin, a lightweight web framework for Java and Kotlin.

Our frontend is written in Javascript using React and is located here: https://github.com/Insanityandme/systemutv-II-frontend

# Install
Our application is divided into two separate parts
+ backend
+ frontend

## Backend
<img src="https://github.com/Insanityandme/my-happy-plants/assets/1380257/e976f1b8-922e-49ce-9d8e-450c451496e0"/> 

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
3. Run Javalin.java and it should look something like this: ![image](https://github.com/Insanityandme/systemutv-II-backend/assets/1380257/03980c76-d2d6-48ba-94a2-3be7ee24764d)
4. Now that the server is running navigate to localhost:7002 to check out our API documentation! ![image](https://github.com/Insanityandme/systemutv-II-backend/assets/1380257/01fa74d0-7c10-41f9-ac39-3c942cc34a25)

## Using terminal
1. Make sure you have maven installed on your computer (SEE: https://www.baeldung.com/install-maven-on-windows-linux-mac)
2. run ```mvn install``` in the root of the project
3. run ```mvn compile``` in the root of the project
4. run ```mvn clean package``` in the root of the project
5. run ```java -jar .\target\MyHappyPlants-1.0-SNAPSHOT-jar-with-dependencies.jar```
6. The server should now be running and should look something like this: ![image](https://github.com/Insanityandme/systemutv-II-backend/assets/1380257/f5db41fd-98fc-4649-89a8-521cb6a91c12)

# Testing 

## Using IntelliJ
1. Go into src/main/testing folder
2. If Mockito and Junit is installed (it usually is included in your IDE or will be installed through Maven)
3. Run all files except Helper.java
4. It should look something like this depending on your editor: 
![image](https://github.com/Insanityandme/systemutv-II-backend/assets/1380257/be9d35ab-a25d-46b4-9530-bed329ff5aee)

## Using terminal
1. Same as with running the server you need to have Maven installed globally on your computer for this to work properly
1. cd into root of the project
2. if you've run ```mvn install``` and ```mvn clean package``` you are good to go.
3. run ```mvn clean test```
4. It should look something like this: ![image](https://github.com/Insanityandme/systemutv-II-backend/assets/1380257/17a3b794-3187-4fba-9633-2b28bf8554b2)


# Frontend
This is the frontend part of MyHappyPlants, it is written in React and acts as a replacement of the JavaFX 
portion of the legacy project we worked on for six weeks our second year of university. 

# Install
1. ```git clone https://github.com/Insanityandme/systemutv-II-frontend.git```
2. Download and install NodeJS: https://nodejs.org/en/download/current
3. ```cd``` into systemutv-II-frontend
4. run ```npm install``` to install all dependencies
5. run ```npm start```
6. The server should now be running at localhost:3000!
7. It should look something like this:
<img src="https://github.com/Insanityandme/systemutv-II-frontend/assets/1380257/87e0fe43-34d5-46ca-b7bf-4e783dd30c62"/> 

# Testing
NOTE: There are two ways to run our tests: By running each file or through the command line

1. Editor: Go into src/Tests and run each file
2. Command line: ```npm test```
3. Press a to run all tests
4. Done!
5. It should look something like this:
6. IDE: ![image](https://github.com/Insanityandme/systemutv-II-frontend/assets/1380257/1ea8df6a-6cde-4c21-a273-24dd83ca59b0)
7. Terminal: ![image](https://github.com/Insanityandme/systemutv-II-frontend/assets/1380257/1d8e51f7-d409-4413-a22d-f4aede84fd50)
8. Sometimes ```npm test``` does not run all 7 test suites, simply rerun and it should catch them all!

# Contact
You are welcome to contact me at bengtegardbook@gmail.com if you have any questions on how to setup this environment.
There might be some mistakes in our installation guide and I apologize for that if that's the case.
