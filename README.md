# DevOps frontend

## Nyt repo

1. lav et nyt github repository med start koden.
2. Gå ind på settings/secrets
3. Klik på 'New secret'
4. indtast 'DOCKERHUB_IMAGENAME' under Name og sæt value til dit image navn og klik 'Add secret'
5. gør dette for følgende 4 værdier:

- Name = DOCKERHUB_TOKEN Value = Access Token som du har oprettet på dockerhub
- Name = DOCKERHUB_USERNAME value = dit dockerhub brugernavn
- Name = TEST_USER Value = test bruger navn
- Name = TEST_PASSWORD Value = test bruger password

## Sonarcloud settings

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

## Cypress testing

1. Opret en 'cypress.env.json' i roden af repo'et
2. Tilføj følgende til filen:
   {
   "TEST_USER": "CHANGEME",
   "TEST_PASSWORD": "CHANGEME"
   }
3. Lav dine tests under cypress/e2e
