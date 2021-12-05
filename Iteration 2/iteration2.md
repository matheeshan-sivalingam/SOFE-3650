# Iteration 2 - Identifying Structures to Support Primary Functionality 
## Step 2: Establish iteration goal by selecting drivers
The goal of this iteration is to address the general architectural concern of identifying structures to support primary functionality. The system's primary use cases are the following: <br>
- UC-1: Account creation
- UC-2: Enter login info
- UC-3: User’s information required (location, sexual orientation, hobbies)
- UC-4: Profile suggestions and matches

[Use Case Descriptions.](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/images/UseCaseDes.png)

## Step 3: Establish iteration goal by selecting drivers
The elements that will be refined in this iteration are the modules located in the different layers defined by the Web application reference architecture created in the last iteration. 

## Step 4: Choose One or More Design Concepts That Satisfy the Selected Drivers
The domain model architecture was the chosen design concept to satisfy the selected drivers for this iteration.
Design Decision and Location | Rationale and Assumptions
------------- | -------------
Utilize the domain model architecture for the application | Using domain model architecture will help create an organized structure for Weeble’s system architecture (CRN-1).
Identify domain objects | Identifying each domain object in the architecture will help us separate the concerns easier (CRN-2).
Define domain components, functions and responsibility from domain objects | Defining each component, function, and responsibility would make it easy to manipulate and understand the elements of each layer.
Use AJAX and Spring framework | As Spring is a Java-based framework, developers will be able to get acquainted and utilize it easily (CRN-3).

## Step 5: Instantiate Architectural Elements, Allocate Responsibilities, and Define Interfaces

Design Decision and Location | Rationale and Assumptions
------------- | -------------
Create an initial domain model | We must define all necessary layers in the system. 
Define components (domain objects) and map with use cases | Analysing the use cases can lead to the defining of domain objects
Decompose domain objects in layers | Will allow any team members to be able to see the rest of the modules, making it easier to split up work among members. 
Connect components using Spring | Aspects are supported, and modules are able to be unit tested (CRN-4). 
Relate framework with a data layer module | The AJAX framework selected will be used for this as it can receive data from the server side  in the background without interfering with anything else. 


## Step 6: Sketch Views and Record Design Decisions
![image](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/images/InitialDomainModel.png)
![image](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/images/DomainObjects.png)
![image](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/images/PrimaryCaseModules.png)

## Step 7: Perform Analysis of Current Design, Review Iteration Goal and Achievement of Design Purpose
Not Addressed | Partially Addressed | Completely Addressed | Design Decisions Made During the Iteration
------------- | ------------- | ------------- | -------------
|||UC-1|Modules Identified
|||UC-2|Modules Identified
|||UC-3|Modules Identified
|||UC-4|Modules Identified
||QA-2||The elements that support the associated use case (UC-1, UC-3) have been identified.
||QA-3||The elements that support the associated use case (UC-1, UC-2) have been identified.
|||CON-1|After account creation, the database is capable of handling up to 10,000 users
||CON-3||The suggestion algorithm had been addressed yet the option to access the profile of those suggested users and set them as a match has not yet been addressed
|||CON-5|Addressed in account creation which cannot occur for user without at least 1 hobby being entered
|||CRN-1|Both the structure type (layered) and the definition of modules within layers of the structure have been addressed
||CRN-3||The Spring framework, which is Java-based, has been chosen for this project.
||CRN-4||While up to 10,000 user information slots can be stored, the traffic output has not been addressed yet
|CRN-6|||User matching has not been addressed yet and comparison algorithm is not yet implemented
