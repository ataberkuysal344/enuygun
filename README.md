#EnUygun Money Transfer System
This project was a challenging one since i did not know %75 of it.I did my best to manage this project. At first i managed to write the java codes and used spring booth app to connect mysql database that i've. I managed to create a MYSQl database and have connected it to my Spring Tools. In the pom file, you can see the dependecies that i have. There are Account, Customer, Money Transfer classes. They all have repository, controller and service. I used JDK 17.
The codes have worked well and connected the MYSQL with the Spring Tools. Then i installed Docker (i did not install it before:) and Postman. I also used Postman before connecting it to the Kubernetes and have created some accounts and customers but i've deleted them before conencting it to Kubernetes ( i did to understand how it works ).Then for kubernetes and docker, Ive created the yaml files for deployment and service, also did the same for MYsql.
Then i ran docker application, and as you can see from the screenshots, the pods are working. I used minikube to connect the database to the containers and clusters, and they worked rapidly.
In the code there will be 2 accounts created from the beginning. I did it because i wanted to check whether the API's are working or not when i hardcode it. I created other Accounts based on my Favorite Anime and my Favorite Guitar.
As you can see from the files, Itadori Yuji has 2 accounts created. One of them is his scholarship account and one them is personal. The main reason was to do this was to  the accounts and customer id will change even though they are used by the same person. Also there is Satoru Gojo, which is also one of the richest in my API's. Gojo will buy a Les Paul which has a 120 dolars of worth (i wish it did have the same value). I thought of gathering them into one but the time i had was limited, since i studied 40 hours in three days to pass my final exam on algorithms.First we create the customer account to have a spesific UUID, then with the given ID from the Postman we are creating our Account which includes Currency, Amount and Our Customer ID.After posting that, your account is online and we can get how much we have by GET command in ACcounts via Postman.
Then with the account id's we can transfer the money to someone in the list.
There 4 cases i checked in the transaction part.You can find them from my screenshots.
1. transaction was successfull, and the money is transferred correctly.
2. UUID was not available, so the money did not get transferred, and the system showed us the error.
3. UUID was too so it gave an error.
4. The money source could not pay the amount of money did so it gave an error.

This hardest part was to conncting the database to the Kubernetes, but with the help of a friend and deep dive of StackOverflow, i think i managed to do that.

the password is 12345678 if it asks.
