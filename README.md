# InterviewAllRevision


# Project Experience according to the resume

Our Workflow Management Platform is a configurable onboarding platform. It can support different types of onboarding, such as client onboarding, member onboarding, Alight user onboarding, or non-Alight user onboarding.

When an onboarding request is created, the system identifies the type of onboarding and creates the corresponding workflow with a predefined set of tasks.

For example, one onboarding type may require document upload, validation, compliance checks and approval, while another type may have a different set of tasks.

Each task has its own status, such as Pending, In Progress, Completed or Failed. The overall onboarding status is tracked based on the completion of the required tasks.

For tasks involving file processing, we use AWS S3 for file storage and Kafka for asynchronous event processing. The Spring Boot services manage the workflow, task status, validations and database operations, while PostgreSQL stores the workflow and task metadata.

So, overall, the platform provides a centralized way to manage and track different onboarding processes through configurable workflows and tasks.

























