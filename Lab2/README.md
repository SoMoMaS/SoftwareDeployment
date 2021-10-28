# SoftwareDeployment
- Created simple node js application with express
- Added unit test with mocha
- Created new pipeline
- Pipeline connected to the Github repo of the simple Node.js project
- Run Build and Deploy jobs --> successful
- Creating a new release pipeline for an azure nodejs service
- Adding an artifact
- Enabling continuous deployment trigger --> for automatic pipeline release in the future commits
- Deploying the release pipline had an error: "No package found with specified pattern: D:\a\r1\a\**\*.zip<br/>Check if the package mentioned in the task is published as an artifact in the build or a previous stage and downloaded in the current job."
- Found a solution on: https://stackoverflow.com/questions/53117244/azure-devops-pipeline-release-error-no-package-found-with-specified-pattern-d
- I had to edit the pipline yaml file by puting the following line at the end of the file: "- task: PublishBuildArtifacts@1"


$(System.DefaultWorkingDirectory)/**/*.zip