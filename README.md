# Gruppe 2 startcode - Frontend

## How to setup the project

The project assumes that you have a backend setup with auth, test users aswell as the joke and scrape endpoints.
Startcode for the backend can be found [here](https://github.com/Paepke-cph/TeamGoldStartCode-Backend)

- Clone this repo
- npm install
- Change backend URL in settings.js - remember '/api'

#### Sonarcloud settings

Steps on sonarcloud.io

- create new project
- encrypt your token with travis(you can use docker for this if you don't want to install local. tip: pull ruby image) and add the token to travis.yml in project root
- Add your new repo to be analyzed.
- disable automatic analyze by sonarcloud.

Steps local

- goto "sonar-project.properties"
- sonar.projectKey=your_project_key
- sonar.organization=the_organisation_you_imported_in_sonarcloud
- sonar.pullrequest.github.repository=your_git_repo
- You're golden...

### TEST

_Cypress_

- Provides UI testing for advanced state management
- TODO add UI testing for the rest of the components
