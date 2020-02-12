# Climb!

## Project summary

### One-sentence description of the project

Climb! is a web application that advances the climbing competition experience by automating the scoring and verification process involved.

### Additional information about the project

**Target Audience**: Event coordinators and competitors in climbing competitions

**Main Functionality**

- Competitors can upload scores
- Competitors can view automatically calculated results
- Competitors can have climbing scores verified digitally
- Competitors can view past competitions and scores
- Competitors can register for competitions

## Installation

### Prerequisites

- Git (v2.21.1)
- Heroku (v7.38.0)
- Node (v12.14.1)
- PostgreSQL (v12.1)

### Dependencies

- React (v6.13.4): Allows for the creation of web components for the frontend
- React Router (v6.13.4): Allows for routing of pages in the frontend
- React Router DOM (v6.13.4): Allows for routing of pages in the frontend
- Axios (v6.13.4): Allows for creating and handling API calls to the backend

### Installation Steps

**Frontend**

Testing the web application on localhost:
1. Navigate to the <code>frontend</code> subdirectory:
<pre>cd frontend</pre>
2. Install necessary dependencies:
<pre>npm install</pre>
3. Start the web server:
<pre>npm start</pre>

Deploying the web application on Heroku:
1. Configure the Heroku deployment:
<pre>
cd ..
heroku login
heroku git:remote -a [my-app-name]
</pre>
2. Push the web application to Heroku:
<pre>git subtree push --prefix frontend heroku master</pre>

## Functionality

Here are our <a href="cs48-climb-frontend.herokuapp.com">frontend</a> and <a href="cs48-climb-backend.herokuapp.com">backend</a> in production.

- Navigate to the homepage.
- Click on "Get Started" or "Sign Up" and create an account. If you already have an account, click on "Log In" and log in.
- Click on "Create Competition" and create a competition. If a competition already exists, click on "Join Competition" and join the competition.
- Click on "Log Scores" and log scores for a given competition and route.
- Click on "View Scores" and view the top 3 scores for a given competition.

## Known Problems

- On the frontend's /log/scores webpage, the JSON response is not formatted properly, so all scores are only shown as a string in the table
- On the frontend, there have been glitches in remembering whether the user is logged in or not.


## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D
