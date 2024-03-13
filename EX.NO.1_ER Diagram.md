# EXP NO 1: ER DIAGRAM CREATION, RELATIONAL MODEL AND SCHEMA GENERATION  
### DATE
## AIM:
<div align="justify">
   To create a ER Diagram for Bank management system or College management system using ERD Plus tool and generate the relational model with schema. 
</div>

## Algorithm
1. Create a login with https://erdplus.com.
2. Create a new ER Diagram with name
3. Create a strong entity, relation and attributes.
4. Create a weak entity, relation and attributes.
5. Specify attributes unique, multivalued and composite attributes.

### ER Diagram 

![Screenshot 2024-03-13 102457](https://github.com/arun1111j/DBMS/assets/128461833/ade97f64-b5a6-4caf-b938-c39ae1434ea7)

### Relational model

![Screenshot 2024-03-13 102503](https://github.com/arun1111j/DBMS/assets/128461833/e13b0fc5-485a-4d8d-906a-f06650a30eed)

### SQL DDL Schema 
```
CREATE TABLE BANK
(
  Code INT NOT NULL,
  Name VARCHAR(100) NOT NULL, -- Assuming the name of the bank can be a string
  Addr VARCHAR(255) NOT NULL, -- Assuming the address of the bank can be a string
  PRIMARY KEY (Code)
);

CREATE TABLE BANK_BRANCH
(
  Branch_no INT NOT NULL,
  Addr VARCHAR(255) NOT NULL, -- Assuming the address of the branch can be a string
  PRIMARY KEY (Branch_no)
);

CREATE TABLE LOAN
(
  Loan_no INT NOT NULL,
  Amount DECIMAL(10, 2) NOT NULL, -- Assuming the amount of the loan can be a decimal number
  Type VARCHAR(50) NOT NULL, -- Assuming the type of loan can be a string
  PRIMARY KEY (Loan_no)
);

CREATE TABLE CUSTOMER
(
  Phone VARCHAR(20) NOT NULL, -- Assuming phone numbers can be stored as strings
  Ssn INT NOT NULL,
  Name VARCHAR(100) NOT NULL, -- Assuming the name of the customer can be a string
  Addr VARCHAR(255) NOT NULL, -- Assuming the address of the customer can be a string
  PRIMARY KEY (Ssn)
);

CREATE TABLE ACCOUNT
(
  Acct_no INT NOT NULL,
  Balance DECIMAL(10, 2) NOT NULL, -- Assuming the balance of the account can be a decimal number
  Type VARCHAR(50) NOT NULL, -- Assuming the type of account can be a string
  PRIMARY KEY (Acct_no)
);
```
## RESULT 
<div align="justify">
Thus the ER diagram was drawn and relational diagram, SQL DDL staements are generated using ERD plus tool.
</div>
