# SoftwareDeployment

## Simple Node app Github Repo: https://github.com/SoMoMaS/TestNodeAPI

## Link to azure website: https://nodesampleproject.azurewebsites.net/

## Link to DevOps project: https://dev.azure.com/110192/nodesampleproject

- Created simple node js application with express
- Added unit test with mocha
- Created new pipeline
- Pipeline connected to the Github repo of the simple Node.js project
- Run Build and Deploy jobs --> successful
- Creating a new release pipeline for an azure nodejs service
- Adding an artifact
- Enabling continuous deployment trigger --> for automatic pipeline release in the future commits
- Deploying the release pipline had an error: "No package found with specified pattern: D:\a\r1\a\**\*.zip<br/>Check if the package mentioned in the task is published as an artifact in the build or a previous stage and downloaded in the current job."
- I needed to add a task for the yaml file to publish and build the artifacts
- Continuous Deployment activated
- Turned on the function which requires me to approve all the releases after changing the source code and pushing to the github repo