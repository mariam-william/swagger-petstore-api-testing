# swagger-petstore-api-testing
A Petstore server sample for API testing using Postman

## To run via command line

- Export [collection](https://learning.postman.com/docs/getting-started/importing-and-exporting-data/#exporting-collections
) from Postman by
  1. Select the more actions icon next to the collection, then select Export
  2. Select Export to download your newly generated JSON file

- If you are using environment variables, you can export [environment variables](https://learning.postman.com/docs/getting-started/importing-and-exporting-data/#exporting-collections
) from Postman by
  1. Select the Environments tab from the left navigation menu.
  2. Select an environment to export.
  3. In the main work area, select the more actions icon, then select Export to download your newly generated JSON file.

- Install [newman](https://learning.postman.com/docs/running-collections/using-newman-cli/command-line-integration-with-newman/) command-line Collection Runner for Postman using this command
`npm install -g newman`

- Open command line in file system and run this command
`newman run mycollection.json`

- If you are using environment variables, you can run this command
`newman run mycollection.json -e myenvironment.json`

## To run via Jenkins
1. Install [Jenkins](https://www.jenkins.io/download/)
2. Go to command line and check if java is installed by running this command `java -version`, if not installed go to this [link](https://www.oracle.com/java/technologies/downloads/#java8) and install java 8
3. Run this command `java -jar "jenkins path"`
4. Copy a password that will appear in command line while installation is in progress to use it later.
5. After Jenkins installation finishes, go to browser and go to [localhost](http://localhost:8080/).
6. Type the password you copied.
7. Setup jenkins.
8. Create a new account for jenkins.
9. Create a new job if no existing jobs in jenkins.
10. Type your item name and choose "Freestyle project".
11. Add project description and choose windows patch command and run this command 

    `newman run https://www.getpostman.com/collections/924928a50fbb116d0409`

13. Click on save then click on Build Now and check the build results.
