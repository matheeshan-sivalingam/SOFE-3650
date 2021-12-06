# SOFE3650 Final Project - Software Architecture Analysis of Weeble 

![Weeble Logo](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/images/weeble_logo.png)

## Group members
Matheeshan Sivalingam (100703887)<br> 
Harvee Sandu (100704514)<br>
Julian Pascual (100707563) <br>
Ashad Ahmed (100745913)<br>
## Table of Contents
- [Project Description](#pd)
- [Functional/Non-Functional Requirements](#fun-requirements)
- [Use Case Diagram](#useCase)
  - [Description](#des)  
  - [Quality Attributes](#qa)
  - [Constraints](#con)
  - [Architectural Concerns](#ac)
- [Iterations](#iter)
- [Appendix](#app)




## <a name = "pd" style="color: black;">Project Description</a>
Weeble is a web application that allows users to match and connect with individuals who share
similar interests and/or hobbies. This application will allow the user to create a profile in which
they can express their preferences, hobbies, and interests. It will then take these parameters into
consideration and find compatible matches that fit the user’s criteria. In comparison to other
dating websites in the market, the algorithm designed for this application will have a strong focus
on prioritizing the hobbies and interests of the user. This software is intended to help facilitate
individuals who are seeking intimate as well as platonic relationships. 

## <a name = "fun-requirements" style="color: black;">Functional/Non-Functional Requirements </a>
### Functional Requirements
1. User must be able to create an account by inputting there first name, last name, email, password, date of birth, and gender.
2. User can only be able to login to website if their inputted username and password matches with the username and password in the database
3. User must be able to specify their gender preference, location, and atleast one hobby.
4. User should only see potential matches that fits their specific criteria (gender preference and hobby)  
5. User must be able to accept or reject potential matches 

### Non-Functional Requirements
1. The website should find and display all potential matches to a user in less than 3 seconds
2. The website should be able to run on all modern browsers (Edge, Google Chrome, Safari, etc)  
3. The database must be able to store atleast 10000 user profiles 
4. The user interface should be intuitive and easy to use 
5. All the user's information must be stored securely into the database. 

## <a name = "useCase" style="color: black;">Use Case Diagram</a>
![image](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/images/UseCaseDiagram.png?)<br>
### <a name = "des" style="color: black;">Description</a>
<br>![image](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/images/UseCaseDes.png?)<br>
### <a name = "qa" style="color: black;">Quality Attributes</a>
![image](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/images/QA.png?)
### <a name = "con" style="color: black;">Constraints</a>
![image](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/images/Constraints.png?)
### <a name = "ac" style="color: black;">Architectural Concerns</a>
![image](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/images/ArchitecturalConcerns.png)


## <a name = "iter" style="color: black;">Iterations</a>
### [Iteration 1 - Establishing an Overall System Structure](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/Iteration%201/Iteration1.md)
### [Iteration 2 - Identifying Structures to Support Primary Functionality](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/Iteration%202/iteration2.md)
### [Iteration 3 - Addressing Quality Attribute Scenario Driver](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/Iteration%203/Iteration3.md)

## <a name = "app" style="color: black;">Appendix</a>
### [Master Document](https://docs.google.com/document/d/1Ztx1glYZJMI7zUGeRQDZ8p5d3o8vcK3YSCOyWBPXVzI/edit?usp=sharing)<br>
### [Presentation slides](https://docs.google.com/presentation/d/1JY9X4QtH4G_LmyMREkuHsE9DJMp2nOsP86n26DD2asU/edit?usp=sharing)
