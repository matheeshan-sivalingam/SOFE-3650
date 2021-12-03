# Iteration 1
## Step 1: Review Inputs
Category | Details
------------- | -------------
Design purpose | The purpose of this application to create a platform that connects people to each other based on their hobbies and interests. This is a greenfield system from a mature domain.
Primary functional requirements  | UC-1: Account creation<br>UC-2: Enter login info<br>UC-3: User’s information required (location, sexual orientation, hobbies)<br>UC-4: Profile suggestions and matches<br><br>[Use Case Descriptions](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/images/UseCaseDes.png).
QA Scenarios |  <table>  <thead>  <tr> <th>QA</th> <th>Importance</th> <th>Difficulty of Implementation</th> </tr> </thead>  <tbody>  <tr>  <td>QA-1</td>  <td>Medium</td> <td>High</td> </tr> <tr> <td>QA-2</td>  <td>High</td> <td>Medium</td> </tr><tr> <td>QA-3</td>  <td>High</td> <td>Medium</td> </tr><tr> <td>QA-4</td>  <td>Medium</td> <td>Low</td> </tr> <tr> <td>QA-5</td>  <td>Low</td> <td>Medium</td> </tr>  </tbody>  </table> From this, QA-2 and QA-3 are choosen as drivers.<br><br>[Quality Attributes](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/images/QA.png).
Constraints|CON-1, CON-3 and CON-5 are of the highest priority so they are selected as drivers<br><br>[Constraints](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/images/Constraints.png).
Architectural Concerns|CRN-1, CRN-3, CRN-4 and CRN-6 are of the highest priority so they are selected as drivers <br><br>[Architectural Concerns](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/images/ArchitecturalConcerns.png).

## Step 2: Establish iteration goal by selecting drivers
**The iteration goal is to achieve the architectural concern of establishing an overall system structure.**
- QA-2: Security
- QA-3: Security
- CON-1: Database must be able to securely store and hold the information of a minimum 10,000 users
- CON-2: Website must be able to support a minimum of 5000 simultaneous users at a single time
- CON-5: The user must have at least one hobby selected to be able to create a profile
- CRN-1: Establish an organized and easy to extend system architecture
- CRN-3: Creation of the product should include Java and MySQL technologies
- CRN-4: Store information of >10k users, maintain traffic of >1000 simultaneous users
- CRN-6: Similarities of hobbies and interests should influence matching significantly

## Step 3: Establish iteration goal by selecting drivers
This is a social network system, so the element to refine is the entire Weeble system. Refinement is performed through decomposition.

## Step 4: Choose One or More Design Concepts That Satisfy the Selected Drivers
Design Decision and Location | Rationale
------------- | -------------
Logically structure the client part of the system using the Web application reference architecture | The web application reference architecture provides cross cutting functionality such as security which would help achieve QA-2, as minimal data would be stored on the user side and all data processing would occur on the server. In addition, the separation of layers addresses CRN-1. <br><br> DISCARDED ALTERNATIVES: <ul><li>Rich Client Application - Cannot be used as Weeble is a web application.</li><li>Rich Internet client app -  Cannot be used due to high loading times (violates QA-1)</li><li>Mobile application - Cannot be used as Weeble must be accessed through a web browser</li></ul>
Build the backend database using MySQL | Take advantage of prior developer experience by using MySQL for the system’s database backend (CRN-3). MySQL is also capable of high performance and can handle large databases (CRN-4).<br><br> DISCARDED ALTERNATIVES: <ul><li>MongoDB (limited experience: CRN-3)</li></ul>
Build the presentation tier and data layer with Java | Java can be used to build web applications. Weeble should use Java, as the developers have experience with this technology (CRN-3).<br><br> DISCARDED ALTERNATIVES: <ul><li>PHP (security concerns: QA-2, QA-3)</li><li>ASP.NET (limited experience: CRN-3)</li></ul>

## Step 5: Instantiate Architectural Elements, Allocate Responsibilities, and Define Interfaces
Design Decision and Location | Rationale
------------- | -------------
Add application facade component to the web application architecture|Implementing the facade component to the web application architecture will provide an extra layer of abstraction between the presentation and business layer.

## Step 6: Sketch Views and Record Design Decisions
![image](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/images/Iteration1Outcome.png)

