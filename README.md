# Applications-of-Threads-and-Semaphores-
An application made in C, to better understand the working of threads and semaphores. 3 new problem statements are proposed and solved them using the concepts mentioned above.

1. Parts of a Car:
Let’s assume a situation where the headquarters of the company can accommodate only 2 of the 3 resources for manufacturing a car at a time. We assume that the three resources are Engine, Chassis and Music System. The 2 resources are supplied to the headquarters and sent to a workshop where the third resource is available. After all the resources are received at the workshop, the car is assembled and is ready to be sold in the market.

Constraints:
• The resources are allocated to the headquarters randomly.
• Only 2 resources are accessed at a time in the headquarters and the third resource is made available in the workshop.


2. Gas Station:
Consider a gas station with three gas pumps, three attenders and a waiting lane that can accommodate four cars. Only 7 cars are allowed inside the station; 3 at the gas pump and 4 in the waiting line. A car will not enter the gas station if 7 there are already 7 cars in the station. Once inside, the car enters the waiting lane (a queue). When an attender is free, the car at the head of the queue drives up to that gas pump and gets served. When a car’s filling is done, any attender can accept the payment, but because there is only one ATM machine, payment is accepted for one car customer at a time. The attenders divide their time among serving cars, accepting payment whilst waiting to do the same.

Constraints:
• The Cars invoke the following functions in order: enterStation, waitInLine, goToPump, pay, exitStation.
• Attenders invoke serveCar and acceptPayment.
• Cars cannot invoke enterStation if the gas station is at capacity.
• If all the three pumps are busy, a car in the wait lane cannot invoke goToPump until one of the cars being served invokes pay.
• The car customer has to pay before the attender can acceptPayment.
• The attender must acceptPayment before the car can exitStation.

3. Cafeteria Problem:
Assume a cafeteria with only one cook during lunch times that puts the food in the trays and puts the trays on a conveyor belt so students can fetch them and eat. The conveyor can take at most 8 trays. If the conveyor is full, the cook sleeps until a tray is fetched. Students come in and fetch their trays. If there are no trays available, they wait until the cook fills a tray and puts it on the conveyor.

Constraints:
• If the conveyor is full, cook sleeps; if not, he fills trays.
• Each student has to be a different thread.
• One student can fetch only one tray at a time.
• Order of the students while fetching a tray is not important.
