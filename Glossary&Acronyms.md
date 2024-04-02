Glossary 
===============================

*This glossary describes the terms and acronyms that will be used to support the management of a financial family application*


### Index with developed terms ###


| Sprint   | TERM                            |       |      Explanation                                                                                                            
|----------|---------------------------------|-------|-----------------------------------------------------------------------------------------------------------------------
| **1st**  | Vat                             |       | An identifier number used for value added tax purposes.                                                                      
| **1st**  | System Manager                  |       | Has the role to manage and design information systems in a variety of settings.                                              
| **1st**  | Family Administrator            |       | Family member with the responsibility to add other family members, create relations between them, get the list of family members, and the categories on the family tree    
| **1st**  | Standard Category               |       | Categories that are already defined and that define the most common categories of family expenses or transactions.  
| **1st**  | ID                              |       | It is an identifier that is assigned to a class and used to identify it in a unique manner.
| **1st**  | Application                     |       | It is a class that is going to deliver responsibilities to the services classes.
| **1st**  | UI                              |       | User Interface
| **1st**  | Controller                      |       | A controller is the first object beyond the UI layer that is responsible for receiving or handling a system operation message.
| **1st**  | Email                           |       | A class that validates the e-mail attribute description.
| **1st**  | emailAddress                    |       | Attribute of the Email class that defines the content of the email.
| **1st**  | emails                          |       | Attribute of the Person class which is an list of emails of that Person 
| **1st**  | Profile                         |       | Representation of the individual of basic information such as name, date of birth, phone, email, VAT number, address, family and ID. 
| **1st**  | Person Service                  |       | Class that is intended to perform operations of the Person class.
| **1st**  | Family Service                  |       | Class that is intended to perform operations of the Family class.
| **1st**  | Category Service                |       | Class that is intended to perform operations of the Person class.
| **2nd**  | withdraw()                      |       | Function that removes money from the account
| **2nd**  | deposit()                       |       | Function that adds money to the account
| **2nd**  | MoneyValue                      |       | Class that encapsulates a numeric value and a currency
| **3rd**  | FamilyRelation                  |       | Given the attributes of the class: the person with _personID_ is "_relation type_" of person with _kinID_
| **3rd**  | RelationType                    |       | As a denomination of the relation type and also the opposite denomination, e.g. parent (denomination) -> child (opposite denomination)
| **5th**  | InDTO                           |       | Is the type of DTO that the Rest Controller receives
| **5th**  | OutDTO                          |       | Is the type of DTO that goes between the Service layer and the Controller layer 
| **5th**  | AssemblerDTO                    |       | Is the type of DTO that the assembler of a JPA object receives


### DTO package convention ###

| DTO name            |   Package                    | Flow direction                              | Example
|---------------------|------------------------------|---------------------------------------------|-------------
| In...DTO            |   indto                      | JSON ---> Controller                        | InPersonDTO
| Out...DTO           |   outdto                     | Service ---> JSON                           | OutPersonDTO
| Primitives...DTO    |   controllertoservicedto     | Controller ---> Service                     | PPersonDTO
| ValueObjects...DTO  |   todomaindto                | Service ---> Domain  &  JPA ---> Domain     | VOPersonDTO


### Deprecated ###

| Sprint   | TERM                            |       |      Explanation
|----------|---------------------------------|-------|-----------------------------------------------------------------------------------------------------------------------
| **2nd**  | A-                              |       | Account id prefix
| **2nd**  | P-                              |       | Person id prefix
| **2nd**  | F-                              |       | Family id prefix
| **2nd**  | M-                              |       | Movement id prefix