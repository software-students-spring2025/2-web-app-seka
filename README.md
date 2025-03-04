# Web Application Exercise

A little exercise to build a web application following an agile development process. See the [instructions](instructions.md) for more detail.

## Product vision statement
Provide a simple platform where job seekers can record their applications, practice mock interviews, and manage a collection of interview questions.

## User stories

As a job seeker, I want to create new job application records so that I can manage them.
As a job seeker, I want to update or delete job application records so that I can keep them accurate.
As a user, I want to view all my job applications in one list so that I can know the overall progress.
As a user, I want to practice mock interview questions so that I can have a better performance later in real interview.
As a user, I want to see scores on my practice sessions so I can track my improvement.
As a user, I want to document questions to a personal collection so that I can revisit them.
As a user, I want to remove questions in my collection so that I can keep the relevance of them.
As a user, I want to create an account so that I can save my personal progress and match it with my account.
As a user, I want to log in and log out so that only me can view my job status.
As a user, I want to reset my password so that I wont be worried about losing my pwd.
As a user, I want to add personal notes to each job application so I can set reminder for key details.
As a user, I want to update answers to questions in my collection so I can revise the answer to make it better. 


## Steps necessary to run the software

Use Docker Compose to boot up both the mongodb database and the flask-app web app with one command:

docker compose up --force-recreate --build ... add -d to run in detached/background mode.
and then docker compose down in a separate terminal window to stop the containers when done.
If you see an error message that a particular port is already in use, select a different port for either the flask-app or mongodb service, as necessary. To do so, edit the first port number for that service in the docker-compose.yml file and try again. E.g., change the flask-app's port to 10000:5000 if you want the flask app to run on port 10000 on your computer. If changing the flask-app port in this way, you must also update the FLASK_PORT setting in the docker-compose.yml file to match.

View the app in your browser:

open a web browser and go to http://localhost:5000 (or change 5000 to whatever port number you used for the flask-app.)

## Task boards

[Link](https://github.com/orgs/software-students-spring2025/projects/82)
