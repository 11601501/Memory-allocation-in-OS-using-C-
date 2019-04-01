# Write a multithreaded program that implements the banker's algorithm. Create n threads that request and release resources from the bank. The banker will grant the request only if it leaves the system in a safe state. It is important that shared data be safe from concurrent access. To ensure safe access to shared data, you can use mutex locks.

Salutation:  Suppose the table for Example:

 

Using:  Need = Max – Allocation
We can get the need table for the bankers:
Need
P	A	B	C		D
P0	0	0	0		0
P1	0	7	5		0
P2	1	0	0		2
P3	0	0	2		0
P4	0	6	4		2
Total	1	13	11		4

A system is in a safe state if the amount of resources needed does not exceed the amount of resources available
 A	B	C		D
Available	1	5		2	0

Yes, the system is in a safe state. The amount of resources needed for either Process 3 or Process 0 to run does not exceed the amount of resources available.

 If Request is  arrives for (0, 4, 2, 0) will be granted because :

A		B	C	D
Need 		0	4	2	0
Available		1	5	2	0
Available - Need		1	1	0	0
