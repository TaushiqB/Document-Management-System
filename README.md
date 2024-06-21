# Document-Management-System
 
To execute: Run dms.py and copy paste the address in browser

Tools : Flask, Jinja, SQL Alchemy, Python, HTML, CSS, JS
Primitive Process:

-All the Institutes/ Departments under the Ministry are using some common file/document movement and approval procedures. The physical movement of such files/ documents has many disadvantages.
-When a document file is under process of approval, the location of the file document where it has been delayed on the way while moving from table to table, is very difficult to trace. The status of a document/ file which has been initiated is not traceable until it returns back to the parent section/ Office.


Object Model: 

-Web server based on Flask
-Template engine based on Jinja
-Database integration based on SQL Alchemy


Process: 

-Created a server using python
-Created a User-friendly environment(webpage) for forwarding, rejection/ approval of documents/ files in e-format
-Updation of document approval status to the end user which promotes the right to information and transparency
-Creating a messages section for direct messaging the end user/ government officers for the more info about rejection.


Hierarchy of approval:

Tahsildar
Head Quarter's Deputy Tahsildar(HQDT)
Regional Inspector (RI)
Village Administrative Officer(VAO)


End User/ Government Officer Experience:
 
-Register in the webpage
-Log in to the webpage
-Customized profile is created
-Files displayed in “documents” section
-File Options:
-Download and View
-Rejection/Approval
-Reason for rejection
-Send and receive private message to/from the end user/government officers
-Log out


E-file:

-There is no chance of missing files, even if they are missed, they can be re-transmitted
-Individual cannot access files since they are securely stored in server’s database
-Secured protocols ensure prevention of tampering of documents
-There is abundance of storage space, since cloud storage is used
-This procedure does not require attendants/ peons/ MTS personnel for the movement of files
