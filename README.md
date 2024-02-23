SQL statements for creating tables in a relational database. Here's a brief explanation of the tables and their relationships:

studentinfo Table:

Stores information about students, including ID, name, contact details, mentor, batch information, etc.
Foreign Key: batchid references the batchinfo table.

taskinfo Table:

Contains information about tasks assigned to students, including task name, associated student, mentor, batch, completion date, etc.
Foreign Keys: studentid references the studentinfo table, and mentorid references the mentorinfo table.

mentorinfo Table:

Holds information about mentors, including ID, contact details, assigned batch, expertise area, etc.

batchinfo Table:

Stores information about batches, including ID, name, total students, mentor, start date, etc.
Foreign Key: mentorid references the mentorinfo table.

queryinfo Table:

Contains information about queries raised by students, including query text, associated student, mentor, notes, tags, etc.
Foreign Keys: studentid and mentorid reference the studentinfo and mentorinfo tables, respectively.

dashboardinfo Table:

Represents the association between students, mentors, and batches.
mockinterviewinfo Table:


Stores information about mock interviews, including student, mentor, and batch details.
Foreign Keys: studentid, mentorid, and batchid reference the studentinfo, mentorinfo, and batchinfo tables, respectively.

AttendanceInfo Table:

Records attendance information for students, including student ID, date, attendance status, and reason for absence.

ResourceInfo Table:

Contains information about educational resources, such as type, title, description, and link.

PerformanceInfo Table:

Stores information about student performance, including assessment type, score, assessment date, and mentor feedback.

PlacementInfo Table:

Records information about student placements, including company name, job title, salary, and start date.

FeedbackInfo Table:

Captures feedback information, including feedback type, text, date, and associated person ID.
Finally, you have established foreign key relationships between the tables using the ALTER TABLE statements.
