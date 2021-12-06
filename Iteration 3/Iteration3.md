# Iteration 3 - Addressing Quality Attribute Scenario Driver 
## Step 2: Establish iteration goal by selecting drivers
**For this iteration, we will be focusing on QA-2:** When the user creates an account and profile, all information should be stored securely into the database. No other user should be able to access this information
## Step 3: Choose One or More Elements of the System to Refine
The following elements that will be refined are the physical nodes were identified during the first iteration:<br><BR>
Database server  

## Step 4: Choose One or More Design Concepts That Satisfy the Selected Drivers
The domain model architecture was the chosen design concept to satisfy the selected drivers for this iteration.
Design Decision and Location | Rationale
------------- | -------------
Implement the Proxy design Pattern | By encrypting the data, it adds an extra layer of security and allows only the intended recipient to be able to read that data
Introduce the Encrypt data tactic by encrypting data when storing into the database | Identifying each domain object in the architecture will help us separate the concerns easier (CRN-2).
  
## Step 5: Instantiate Architectural Elements, Allocate Responsibilities, and Define Interfaces
Design Decision and Location | Rationale
------------- | -------------
Implement Encrypt tactic using Transparent Data Encryption (TDE) architecture  | Implementing TDE architecture encrypts the database with the database encryption key and key encryption key. This fulfills QA-2 as it provides further security and ensures that the data is securely stored in the database      
Deploy protection proxy design pattern by implementing a proxy interface that accesses and make requests to the database  | Deploying the protection proxy interface allows the system to check if the Trans Object/resource has the appropriate authorization to access the data. By doing this, we ensure that only specific objects/resources have access to the data  
  
## Step 6: Instantiate Architectural Elements, Allocate Responsibilities, and Define Interfaces
  
