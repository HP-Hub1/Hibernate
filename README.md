A Java project demonstrating how to interact with a MySQL database using Hibernate ORM.

The project covers:
- Mapping Java entities to database tables (Students, Courses, Teachers, Subscriptions, PurchaseList)
- Creating a new table `LinkedPurchaseList` from data in the `PurchaseList`
- Using a composite primary key (`student_id` + `course_id`) via `@EmbeddedId`
- Auto-generating and updating tables using Hibernate schema tools
- Populating the database using an SQL dump

Technologies Used

- Java 17+
- Hibernate ORM
- MySQL
- Maven
- JPA Annotations
- Lombok

Features

- Full entity mapping using JPA annotations
- Relationships between entities using `@OneToMany`, `@ManyToOne`, etc.
- Composite key implementation using `@Embeddable` and `@EmbeddedId`
- Conversion of purchase data to `LinkedPurchaseList` entries using real `student_id` and `course_id` references
- Auto-schema update based on entity classes

How to Run

1. Create a new MySQL database (e.g., `sqlandhibernate`)
2. Import the provided `purchase_list.sql` dump into the database
3. Set up your database credentials in `hibernate.cfg.xml`
