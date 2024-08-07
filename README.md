# To-Do List Application

This project is a web-based To-Do list application designed to help users efficiently manage their tasks. Built with a focus on simplicity and usability, the application allows users to create, read, update, and delete (CRUD) tasks seamlessly.

### User Interface Snapshots:
_insert ss_ 
- Create Tasks: Users can add new tasks with descriptions.
- Read Tasks: The main interface displays a list of all tasks, including completion status.
- Update Tasks: Users can edit task details.
- Delete Tasks: Tasks can be permanently removed from the list.

## 👨‍💻 Team Description

Our team consisted of three members, each with the following responsibilities:

Aaron Brooker: 
- Implement backend code
- Write tests
- Implement linting checks
- Implement code formatting
- Review pull requests
- Contribute to documentation

Alex McDonald:
- Manage database
- Implement backend code
- Write tests
- Review pull requests
- Contribute to documentation

Azra Mukadam:
- Design user interface
- Write tests
- Review pull requests
- Contribute to documentation

The workload was split evenly between each member of the team, with different primary focuses in different areas, but all areas being crucial to the development of the project. Therefore, the contribution was 33% from each team member.

## 🛠 Tools Used

In the development of our To-Do application, we utilised a variety of tools to ensure high-quality code, effective project management, and comprehensive testing. Below is a detailed list of the tools we used across different aspects of the project:

### Version control
Git: For tracking changes in the source code during development.
GitHub: As the remote repository for collaboartion, code reviews, and issue tracking.

### Database
MySQL: As the relational database management system for storing user data and tasks.

### Testing
Pytest: For unit and integration testing of Python code to ensure functionality and reliability.
Cucumber/Gherkin: For behavior-driven development (BDD), allowing us to write tests in a human-readable format.

### Test Code Coverage
Coverage.py: To measure the amount of Python code tested by our test suites and identify untested parts of the application.

### Frameworks/Libraries
Pydantic: For data validation and settings management using Python type annotations.
Flask: As the lightweight web framework for the Python backend to handle API requests.
Docker: 

### Linters
Black Formatter: For code formatting to ensure a consistent code style across the project.
Mypy: For static type checking to identify type errors in Python code.

### Project Management Tools
Kanban Board: Used for tracking tasks, managing project progress, and organising work in a visual format. It provided clear visibility into the workflow and facilitated dynamic task allocation.
_insert ss_

### Performance and Accessibility Audit
Google Lighthouse: For auditing the performance, accessibility, and best practices of the web application, ensuring optimal performance and user experience.

### Continuous Integration/Continuous Deployment (CI/CD)
GitHub Actions: For automating the testing and deployment processes, ensuring continuous integration and deployment of code changes. This tool helped maintain code quality and facilitated the smooth release of new features.

## 📑 Running the Application

1. Clone the repository
2. Run the required packages for development in the `requirements-dev.txt` file
```bash
python -m pip install -r requirements-dev.txt
```
3. In the terminal run the following to bring up both the database and webserver:
```
docker-compose up --build
```
4. You should be given a localhost URL, click the URL to run

### How to use the application:
_How to create, update, read, and delete tasks_

## 🚦 Project Workflow

### Project Management Strategies
In the development of our To-Do application, we employed Agile methodologies, specifically utilising the Kanban framework. This approach provided a flexible and efficient way to manage our workflow, prioritise tasks, and ensure continuous delivery of valuable features.

### Agile Practices

- Kanban Board:
We used a Kanban board to visualise the workflow and track the progress of tasks in real-time. The board included columns such as "To Do," "In Progress," "Peer Review," and "Done." This visibility allowed team members to easily see what others were working on and identify tasks that needed attention.

- Daily Stand-Ups:
Daily stand-up meetings were held every morning to ensure team alignment and facilitate communication. During these brief meetings, each team member discussed:
  - What they worked on the previous day.
  - What they planned to work on that day.
  - Any blockers or challenges they were facing.
These stand-ups helped in identifying potential issues early and provided a platform for quick feedback and support.

- Quick Feedback Loop:
Before official pull requests (PRs) were made, we conducted informal code reviews and demonstrations during stand-ups. This practice allowed for immediate feedback and rapid iteration, ensuring that potential issues were addressed promptly and reducing the need for extensive revisions during the formal review process.

- Kanban for Visibility and Flexibility:
The Kanban board was pivotal in providing clear visibility into the workload and progress of each team member. It facilitated dynamic task allocation, enabling team members to pick up tasks that needed to be done without waiting for specific assignments. This flexibility ensured that the team could adapt quickly to changing priorities and workload demands.

### Ceremonies and Retrospectives

- Sprint Planning:
Although we followed a Kanban approach, we incorporated elements of sprint planning to set goals and prioritise tasks for the upcoming week. During these sessions, we reviewed the backlog, selected high-priority items, assigned items to team members, and moved them into the "To Do" column on the Kanban board.

- Retrospectives:
At the end of each week, we conducted retrospectives to reflect on our processes and performance. During these sessions, we discussed what went well, what could be improved, and any lessons learned. The retrospective insights were then used to make iterative improvements to our workflow and practices.

## 🧪 Test Methodologies and Tools
_ss of evidence of tests being run & need to complete_

## 💻 Coding Best Practices
_ss of test suite results_

### Consistent Code Style:
   - **Formatting:** We used Black for code formatting to ensure a consistent code style across the project. This minimised style-related discrepancies and made the code easier to read and review.
   - **Linting:** We used Pylint for Python to catch potential errors and enforce coding standards. This helped in maintaining high code quality and avoiding common pitfalls.

### Type Checking:
   - **Mypy:** We employed Mypy for static type checking in Python. This allowed us to catch type-related errors early in the development process, improving code reliability and reducing runtime errors.

### Documentation:
   - **README:** A comprehensive README file was maintained, providing an overview of the project, setup instructions, and usage guidelines.

### Modular Code:
   - **Separation of Concerns:** We ensured that our code was modular, with distinct separation of concerns. This meant separating business logic from presentation logic and database interactions.
   - **Reusable Components:** We created reusable components and functions to avoid code duplication and promote reusability.

### Version Control:
   - **Git:** We used Git for version control, ensuring that all changes were tracked and could be reverted if necessary. Each feature or bug fix was developed in its own branch and merged back into the main branch after review.

### Code Reviews:
   - **Pull Requests:** We used pull requests (PRs) to review code before merging it into the main branch. Each PR was reviewed by at least one other team member to ensure code quality and catch potential issues.

### Testing:
   - **Automated Tests:** We wrote unit tests, integration tests, and end-to-end tests to ensure our code worked as expected. Testing was an integral part of our development process.

### CI Pipeline

We set up our Continuous Integration (CI) pipeline to automate testing and deployment processes. Here’s how we configured our CI pipeline:

1. **GitHub Actions:**
   - We used GitHub Actions for our CI/CD pipeline. It allowed us to automate the running of tests and deployment processes whenever code was pushed to the repository.
   - **Workflow Configuration:** We created a GitHub Actions workflow folder (`.github\workflows`) that consisted of two files to be executed, one to run a lint test, and the other to run the tests, for each CI/CD run.

2. **CI Workflow:**
   - **Build:** The workflow started by setting up the necessary environment, including installing dependencies for both the backend and frontend.
   - **Linting:** The next step involved running linters to check for coding standard violations.
   - **Testing:** We ran our test suites using Pytest. This step ensured that all new code passed existing tests and that no new bugs were introduced.
   - **Deployment:** Upon passing all tests, the code was automatically deployed to our staging environment for further manual testing and validation.

3. **Snapshots of Test Suite Results:**
   _insert ss_

### Pull Request Strategies

1. **Branching Strategy:**
   - We had a main branch which was the production-ready branch.
   - Each feature that was being added would be developed in it's own branch with a name to describe what the feature being added was.

2. **Creating Pull Requests:**
   - Each feature or bug fix was developed in its own branch.
   - Once the development was complete, a pull request (PR) was created to merge the feature branch into the `main` branch.
   - The PR included a description of the changes, references to related issues, and screenshots if applicable.

3. **Code Review Process:**
   - At least one team member reviewed each PR. The review focused on code quality, adherence to coding standards, potential bugs, and overall implementation.
   - Feedback was provided directly within the PR, and the author made necessary changes.
   - Once the PR was approved, it was merged into the `main` branch.

4. **Automated Checks:**
   - GitHub Actions ran automated checks on each PR, including linting, and testing.
   - Only PRs that passed all checks, and had an approved review were eligible for merging.

## ⚖ Standards

### IEEE 730: Software Quality Assurance Plans

IEEE 730 is a standard developed by the Institute of Electrical and Electronics Engineers (IEEE) that outlines the requirements for creating and maintaining software quality assurance (SQA) plans. The standard provides a comprehensive framework to ensure that software products meet quality expectations and adhere to specified requirements.

#### Reasons for Choosing IEEE 730:
1. Comprehensive Framework: IEEE 730 offers a well-structured and detailed framework for ensuring software quality, covering all critical aspects of the software development lifecycle.
2. Industry Recognition: Being an internationally recognised standard, it provides credibility and assurance to stakeholders regarding the quality and reliability of our software.
3. Alignment with Best Practices: Adopting IEEE 730 helps align our processes with industry best practices, ensuring a systematic approach to quality assurance.
4. Risk Management: The standard emphasizes identifying and mitigating risks, which is crucial for delivering a reliable and robust application.

#### Key Features of IEEE 730 Applied in Our Project:

1. Quality Objectives and Criteria:
   - We defined clear quality objectives and criteria for the To-Do application. This included setting specific goals for functionality, usability, performance, and security. These objectives guided our development and testing efforts to ensure the final product met the desired standards.

2. Organisational Roles and Responsibilities:
   - The standard emphasizes the importance of clearly defining roles and responsibilities. In our project, we designated specific team members for roles such as quality assurance manager, testers, and developers. This clear delineation of responsibilities ensured accountability and streamlined the quality assurance process.

3. Software Reviews and Audits:
   - IEEE 730 advocates for regular reviews and audits of the software and its development process. We conducted regular code reviews, design reviews, and audits to ensure compliance with quality standards. These reviews helped identify issues early and maintained the overall quality of the application.

4. Verification and Validation:
   - Verification and validation are crucial components of the IEEE 730 standard. We implemented comprehensive testing strategies, including unit testing, integration testing, and end-to-end testing, to verify that the software met its requirements. Validation ensured that the application fulfilled user needs and expectations.

5. Risk Management:
   - The standard includes provisions for identifying and managing risks throughout the software development lifecycle. We conducted risk assessments to identify potential issues that could impact the project's success. Mitigation plans were developed and implemented to address these risks proactively.

6. Documentation:
   - Proper documentation is a key aspect of IEEE 730. We maintained thorough documentation through the README file which covered the applications features, usage, and the quality assurance plan.

7. Continuous Improvement:
   - The standard encourages continuous improvement of processes and practices. We held regular retrospectives to evaluate our workflows and identify areas for improvement. Feedback from these sessions was used to refine our development and quality assurance processes continuously.


### ISO/IEC 25010: Systems and Software Quality Requirements and Evaluation (SQuaRE)

ISO/IEC 25010 is an international standard that defines a model for software product quality and quality in use. It provides a framework for evaluating software quality through a set of characteristics and sub-characteristics that describe the software's functionality, reliability, usability, efficiency, maintainability, and portability.

#### Reasons for Choosing ISO/IEC 25010:
1. Comprehensive Quality Model: ISO/IEC 25010 offers a detailed quality model that covers various aspects of software quality, making it suitable for evaluating complex software systems.
2. Industry Acceptance: Being an internationally recognized standard, it ensures that our quality assurance practices align with global best practices and industry norms.
3. Focus on User Experience: The standard emphasises quality in use, ensuring that the software meets user needs and provides a satisfactory experience.
4. Structured Evaluation: It provides a structured approach to assess and improve software quality, helping us systematically address potential issues.

#### Key Features of ISO/IEC 25010 Applied in Our Project:

1. Quality Characteristics and Sub-Characteristics:
   - We utilised the some quality characteristics defined by ISO/IEC 25010 to guide our quality assurance efforts:
     - Functional Suitability: Ensured that the To-Do application provided the necessary functionality and features as required by users.
     - Usability: Prioritised user interface design and user experience, ensuring the application was easy to use and intuitive.
     - Reliability: Implemented measures to ensure the application was available, stable, and recoverable in case of failures.
     - Maintainability: Made the codebase modular and documented to facilitate easy updates and maintenance.

2. User-Centered Design:
   - The standard emphasises understanding user needs and incorporating their feedback. We conducted user research and usability testing to ensure the application met user expectations and provided a positive experience.

3. Evaluation and Measurement:
   - ISO/IEC 25010 provides guidelines for evaluating and measuring software quality. We developed key performance indicators (KPIs) and metrics to assess each quality characteristic, using tools and techniques such as load testing, security audits, and usability testing.

4. Continuous Monitoring:
   - We established processes for continuous monitoring and assessment of software quality. This involved regular testing, performance monitoring, and user feedback collection to identify areas for improvement.

5. Risk Management:
   - The standard includes provisions for identifying and mitigating risks related to software quality. We conducted risk assessments and implemented mitigation strategies to address potential issues that could impact the quality of the To-Do application.

6. Documentation and Reporting:
   - Proper documentation was maintained for all quality-related activities, as documented in this README.

7. Feedback and Improvement:
   - We held regular retrospectives and feedback sessions to review the quality of the software and the effectiveness of our processes. Insights from these sessions were used to continuously refine and improve our quality assurance practices.

## 🎭 Performance and Accessibility Audit
_ss of results & need to complete_






