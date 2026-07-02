Smart Lender - Sample Project Documentation

1. Project Overview
Project Name: Smart Lender
Task Name: Entity Relationship Diagram (ERD) Specification & System Architecture
Submitted By: Lahari (LL)
Objective: To design an automated database and machine learning system that evaluates loan applications, assesses financial risk, and predicts loan approval status.

2. Database Architecture (Schema Specification)
The Smart Lender application maps out data management across 6 core structured entities:
- USER: Manages secure login credentials and access authentication.
- APPLICANT_PROFILE: Stores personal applicant demographics linked to a unique user.
- CREDIT_HISTORY: Tracks financial risk profiles, background checks, and outstanding debts.
- LOAN_APPLICATION: Evaluates individual/co-applicant income and requested amount.
- MODEL: Manages internal ML pipeline references like XG Boost, KNN, Random Forest.
- PREDICTION_RESULT: Connects with application feeds to display approval/rejection outputs.

3. System Workflow
- User Authentication: The client logs in via secure USER credentials.
- Profile & Financial Check: The system retrieves APPLICANT_PROFILE and checks credit history flags.
- Application Intake: The user submits financial variables through the LOAN_APPLICATION interface.
- Machine Learning Inference: The data passes into the trained MODEL pipeline (XG Boost).
- Decision Output: The final approval status is saved in PREDICTION_RESULT and displayed to the user.
