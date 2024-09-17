#### Database Management Notes

Problems with traditional File System:
  Organization
  Redundancy 
  Isolation
  Inconsistency
  Atomicity
  Integrity
  Security

ACID - Atomicity, Consistency, Isolation, Durability
● Atomicity – This property ensures that either the transaction occurs completely or it does not occur at all.
● Consistency –  It ensures that the database remains consistent before and after the transaction
● Isolation –  This property ensures that multiple transactions can occur simultaneously without causing any inconsistency. 
 The resultant state of the system after executing all the transactions is the same as the state that would be achieved if the transactions were executed serially one after the other.
● Durability  - This property ensures that all the changes made by a transaction after its successful execution are written successfully to the disk. It also ensures that these changes exist permanently and are never lost even if there occurs a failure of any kind.

The order in which the operations of multiple transactions appear for execution is called as a
schedule. Serializability is a concept that helps to identify which non-serial schedules are correct and will
maintain the consistency of the database.
● Conflict Serializability - If a given non-serial schedule can be converted into a serial schedule by swapping its non-conflicting operations, then it is called a conflict serializable schedule.
● View Serializability - If a given schedule is found to be viewed as equivalent to some serial schedule, then it is called a view serializable schedule.





2 tier: Client and Server 
3 tier: Client and Application and Server

Schema: Logical representation of databse

Keys: Foreign, Candidate, Alternate, Superkey, Primary, Composite, Artificial

ER Model

Normal Forms

Functional Dependence: A functional dependency X → Y is said to be trivial if and only if Y ⊆ X. Thus, if RHS of a functional dependency is a subset of LHS, then it is called a trivial functional dependency.

Sigma, Pi, Union, Intersection etc query optimization

Relational Calculus
![image](https://github.com/user-attachments/assets/0062c2bc-bc26-4767-99a9-f8e39b47ff3f)


Types of joins:
Inner join - Only what we want to consider

Decomposition of a Relation:
The process of breaking up or dividing a single relation into two or more sub relations is called the decomposition of a relation.
Properties of Decomposition:
● Lossless Decomposition - Lossless decomposition ensures - No information is lost from the original relation during decomposition. When the sub relations are joined back, the same relation is obtained that was decomposed.
● Dependency Preservation - Dependency preservation ensures - None of the functional dependencies that hold on the original relation are lost. The sub relations still hold or satisfy the functional dependencies of the original relation.

Normalization:
In DBMS, database normalization is a process of making the database consistent by-
● Reducing the redundancies
● Ensuring the integrity of data through lossless decomposition

1NF - Phone Number (No multivalued columns. Only Atomic Columns)
2NF - StudentNoCourseNo CourseFee (No Partial Dependency)
3NF - STUD_NO -> STUD_STATE but STUD_STATE -> STUD_COUNTRY (No transitive dependency)

Transaction is a single logical unit of work formed by a set of operations.
Transaction States:
● Active State ● Partially Committed State ● Committed State ● Failed State ● Aborted State ● Terminated State

![image](https://github.com/user-attachments/assets/0dface0b-ccf0-4584-abcb-ff48f6de1749)

DDL: DDL is short name of Data Definition Language, which deals with database schemas and descriptions, of how the data should reside in the database.
DML: DML is short name of Data Manipulation Language which deals with data manipulation and includes most common SQL statements such SELECT, INSERT, UPDATE, DELETE, etc., and it is used to store, modify, retrieve, delete and update data in a database.
DQL: DQL statements are employed to conduct inquiries on the information contained in schema objects. The required data is retrieved according to the query using Data Query Language (DQL) commands.
DCL: DCL is short name of Data Control Language which includes commands such as GRANT and mostly concerned with rights, permissions and other controls of the database system.
TCL: TCL is short name of Transaction Control Language which deals with a transaction within a
database.

