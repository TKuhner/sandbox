need database

# CUSTOMER TABLE
id (auto_increment)
first name - primary key
last name - primary key
email address - string
shipping address - string
company (id)? Foreign Key (Company_id) references (company(id))
equipment make
equipment model
serial number
## should equipment be tied to customer specifically?
pros - keeps record of customer products 
cons - if customer leaves company, they don't bring equipment with them
verdict - probably not going to have make model sn tied to customer



# COMPANY TABLE
id (auto_increment) Primary key
name primary key
billing address


# TICKET TABLE
header ()
customer id Foreign key (Customer_id) references customer(id)
customer name - Foreign key customer_first_name + " " + customer_last_name references customer_first_name +
company id - foreign key company_id references company(id)
Company name - foreign key company_name references company(name)
equipment make - varchar(30)
equipment model - varchar(30)
serial number - varchar(30)
Symptom - varchar(30)
description string
creation date
comments w/ timestamps
delete comments as needed (employee privileges?)






# Functionality - concepts
Customer registers account, tied to a company (display list of added companies/allow them to create a company if it's not in the database?)
Customer creates/fills out ticket
populate equipment from their list of products? (probably not given cons)
don't handle customer products and let them report everything in the ticket?

Employees can see list of tickets (opened/closed)
Employees click on ticket and information populates targeted area
Employee will need search functionality for open tickets (can come later)
Allow employee communication with customer via email? 



# Pages needed
Company home page
Customer account/tickets page
Employee page to see tickets

# .Net  sdk link
https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/sdk-8.0.100-windows-x64-installer
direct link: https://download.visualstudio.microsoft.com/download/pr/93961dfb-d1e0-49c8-9230-abcba1ebab5a/811ed1eb63d7652325727720edda26a8/dotnet-sdk-8.0.100-win-x64.exe

