# DevOps frontend

#### Sonarcloud settings

Steps on sonarcloud.io

- Click on plus sign and choose 'Analyze new project'
- Find your project, click and click again on 'Set Up'
- Click on analyze with Github Actions
- Add the sonarcloud tokens
- Ignore the changes to the github actions to yml file
- Edit the sonar-project.properties file locally and overwrite the following settings:

1. sonar.projectKey
2. sonar.organization

- you are done

### TEST

_Cypress_

- Provides UI testing for advanced state management
- TODO add UI testing for the rest of the components
