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


