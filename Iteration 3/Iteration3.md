# Iteration 3 - Addressing Quality Attribute Scenario Driver 
## Step 2: Establish iteration goal by selecting drivers
**For this iteration, we will be focusing on QA-2:** When the user creates an account and profile, all information should be stored securely into the database. No other user should be able to access this information
## Step 3: Choose One or More Elements of the System to Refine
The following elements that will be refined are the physical nodes were identified during the first iteration:<br><BR>
Database server  

## Step 4: Choose One or More Design Concepts That Satisfy the Selected Drivers
Design Decision and Location | Rationale
------------- | -------------
Introduce the Encrypt data tactic by encrypting data when storing into the database | By encrypting the data, it adds an extra layer of security and allows only the intended recipient to be able to read that data
Implement the Proxy design Pattern | By implementing this design pattern, we are able to create an extra layer of security between the client and server. This will provide protection to sensitive user information.

  
## Step 5: Instantiate Architectural Elements, Allocate Responsibilities, and Define Interfaces
Design Decision and Location | Rationale
------------- | -------------
Implement Encrypt tactic using Transparent Data Encryption (TDE) architecture  | Implementing TDE architecture encrypts the database with the database encryption key and key encryption key. This fulfills QA-2 as it provides further security and ensures that the data is securely stored in the database      
Deploy protection proxy design pattern by implementing a proxy interface that accesses and make requests to the database  | Deploying the protection proxy interface allows the system to check if the Trans Object/resource has the appropriate authorization to access the data. By doing this, we ensure that only specific objects/resources have access to the data  
  
## Step 6: Sketch Views and Record Design Decisions
![image](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/images/Deployment%20Diagram1.png)
![image](https://github.com/matheeshan-sivalingam/SOFE3650-WeebleSoftwareArchitecture/blob/main/images/Sequence%20Diagram1.png) 
  
## Step 7: Perform Analysis of Current Design, Review Iteration Goal and Achievement of Design Purpose
Not Addressed | Partially Addressed | Completely Addressed | Design Decisions Made During the Iteration
------------- | ------------- | ------------- | -------------
UC-1||||Not addressed
||UC-2||Implementing the elements can partially be used to secure the login process.
||UC-3||Implementing the elements can ensure that user data is secured 
UC-4||||Not addressed
|||QA-2|By utilizing the elements , QA-2 can be achieved as TDE ensures that the data is stored securely and protection proxy prevents unauthorized access
QA-3||||Not addressed
||CON-1||Implementing the elements ensures that the data is securely stored
CON-3||||Not addressed
CON-5||||Not addressed
CRN-1||||Not addressed
CRN-3||||Not addressed
CRN-4||||Not addressed
CRN-6||||Not addressed
