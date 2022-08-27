[Click Here](http://udagram-frontend2.s3-website-us-east-1.amazonaws.com/) to get the URL of the Udagram deployed Application

## Diagram of APP process
![image](https://user-images.githubusercontent.com/77749264/187027541-eb42ae13-379e-445f-b00e-07529f85aab7.png)
## Diagram of Deploy Process

[CircleCi] - Connect to GitHub -> [ Github ] - Send Data -> [ CircleCi ] - Build Data & Deploy -> [AWS S3] & [EB Environment] -> Return Data to servers


### Pipeline process
  
  * This is a description of the config.yml file
  
    - **orbs** are the services that we need inside our project such as nodeJs , AWS CLI and EB CLI.
    - **jobs** are a series of commands that has inner detailed steps such as the build job.
    - **workflow** is the order of execution of the jobs we created.

  * first we build the project by running docker as virtual machine to run our project on
  * then we start installing node, API dependencies, Frontend dependencies we lint our frontend code and then start building both the API and Frontend
  * then we hold the workflow untill the approval from CircleCi pipeline to start deploying
