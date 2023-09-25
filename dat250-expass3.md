# Assignment 2 MongoDB

## Validation for the installation of the package 
I followed the instructions provided when to validate the Mango package before installing it. 
I chose to validate the package using the provided PGP signature. I cose this method since it 
provides the strongest guarantees by checking both the integrity and the authenticity of the file. 
I downloaded the binaries for the 4.4.24 version of MongoDB. I found the files on the MongoDB Download Center. 
I then downloaded the public signature for the same version of MongoDB. I then Downloaded and imported the key file
as instructed, and lastly I verified the MongoDB installation file:
![MongoDB installation verification](bilder/innlevering3/Package_validation.png)

The english translation of the message retured is:
gpg: Signature made Wed Jun  5 03:17:20 2019 EDT
gpg:                using RSA key 4B7C549A058F8B6B
gpg: Good signature from "MongoDB 4.4 Release Signing Key <packaging@mongodb.com>" [unknown]

I also got the message:
gpg: WARNING: This key is not certified with a trusted signature!
gpg:          There is no indication that the signature belongs to the owner.
Primary key fingerprint: E162 F504 A20C DF15 827F  718D 4B7C 549A 058F 8B6B

It was mentioned in the instructions that this could happen becuse the signing key in my local trustdb is not 
trusted. Yet the package is in fact properly signed, so I assume that the downloaded package is valid and can be trustesd. 

After installing the package on my computer, I added MongoDB to PATH on my machine, and did a quick check of the version that I had installed:
![MongoDB version](bilder/innlevering3/Mongo-shell.png)

I ran the Mongo Shell, and got familiar with some commands. In the image below I have created a database that is called assign3DB, that I used when working through the tutorials provided in ths assignment.

![Mongo shell](bilder/innlevering3/navigate-mongoShell.png)

## Experiment 1: MongoDB CRUD operations
In this part of the assignment, I followed the tutorials provided about CRUD operations. 

### Insert documents 
![Insert](bilder/innlevering3/Insert.png)

### Query documents
![Query](bilder/innlevering3/Query.png)
![Query with and/or](bilder/innlevering3/Query_and_or.png)

### Update documents
![Update one document](bilder/innlevering3/update_one.png)

### Remove documents
![Delete](bilder/innlevering3/Delete.png)

### Bulk write operations
![Bulk write operations](bilder/innlevering3/bulk-operations.png)

## Experiment 2: Aggregation
In this part of the assignment, I worked my way through the examples in the tutorial about map reduction. 
I developed a new map function that provides the quantity of items purchased by each customer for every item they bought. This function could offer valuable insights into the buying patterns of customers and potentially serve as a tool for monitoring inventory levels.

![Map reduction](bilder/innlevering3/map_reduce.png)




