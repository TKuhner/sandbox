need database

CUSTOMER TABLE
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



COMPANY TABLE
id (auto_increment) Primary key
name primary key
billing address


TICKET TABLE
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






Functionality - concepts
Customer requests repair assistance
Customer creates/fills out ticket
populate equipment from their list of products?
don't handle customer products and let them report everything in the ticket?

Employees can see list of tickets (opened/closed)
Employees click on ticket and information populates targeted area
Employee will need search functionality for open tickets (can come later)



Pages needed
Company home page
Customer account/tickets page
Employee page to see tickets

