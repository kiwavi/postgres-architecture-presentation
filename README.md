# Presentation summary and highlights

### This presentation was given at the Nairobi Linux Users group meetup on 4th April 2026

Like most other Database Management Systems, Postgres has the following key components:

* Client Communications Manager.
* Process Manager
* Relational Query Processor
* Transactional Storage Manager
* Shared Components

The presentation goes through all the components, showing how Postgres implements each. 

At the end of the presentation, you get a high-level understanding of the whole process a given query goes through. 

You will learn about how processes are managed through the process-per-worker model, and why the resultant drawbacks makes it necessary to use a connection pooler. 

You will also learn enough for you to realize what's happening when you run an `explain analyze` statement on a query. When you see a `gather merge` what does that mean?

Postgres is ACID-compliant, and the presentation shows you how this happens. To achieve durability, for example, the role of the Write Ahead Log is highlighted. 

How does Postgres control where data is stored and when it is stored? The presentation introduces you to some interesting and exciting concepts. 

Find the presentation [here](https://github.com/kiwavi/postgres-architecture-presentation/blob/main/Postgres_Architecture_Presentation-2.pdf) 

For further reading, you can look into the following resources:

* [Postgres Docs](https://www.postgresql.org/docs/current/overview.html)
* [Architecture of a Database System ](https://www.google.com/url?sa=t&source=web&rct=j&opi=89978449&url=https://db.cs.berkeley.edu/papers/fntdb07-architecture.pdf)
* [Serializable Snapshot Isolation in PostgreSQL](https://www.google.com/url?sa=t&source=web&rct=j&opi=89978449&url=https://arxiv.org/abs/1208.4179)
