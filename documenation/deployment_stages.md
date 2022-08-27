# Deploy proccess stages

### 1) Database
testing the database connection at aws RDS
![image](https://user-images.githubusercontent.com/77749264/187028010-f65803a4-3edd-4627-8a82-ad6db1896d22.png)

----

### 2) s3 Bucket
After S3 Bucket creation and setting the Static website Enabled
![image](https://user-images.githubusercontent.com/77749264/187028084-dde0ac81-5994-44b7-ba28-1552969f520d.png)


----

### 3) ElasticBeanstalk
#### Adding Environment variables to the ElasticBeanstalk after creation
Include all the needed variables to connect DB
![image](https://user-images.githubusercontent.com/77749264/187028118-e6664033-fa4a-4641-9ea1-6207bc868b31.png)
![image](https://user-images.githubusercontent.com/77749264/187028126-a647e7c1-2c10-49c3-b4ea-398ef0c19ea1.png)


----

#### Checking the ElasticBeanstalk health after adding all variables
checking the EB health after adding the Environemts to connect DB
![image](https://user-images.githubusercontent.com/77749264/187028142-4cd23ebe-d151-433c-9952-f7312aa8b352.png)


### 4) BackEnd Runtime
Checking the URL of the BackEnd server ( **[Live link to server](http://udagram-api-dev.eba-arx29nrv.us-east-1.elasticbeanstalk.com/)** )
![image](https://user-images.githubusercontent.com/77749264/187028168-094202aa-b374-4794-bd0f-e00d171844f6.png)

### 5) FrontEnd connected with BackEnd
Connecting to the S3 website after connecting API with FrontEnd and DB
![image](https://user-images.githubusercontent.com/77749264/187028308-ec695ce6-b769-4ee3-9d57-77a34a20a48b.png)

### 6) Create the Github Repo
Add all files into repo after build and commit it to github 
![image](https://user-images.githubusercontent.com/77749264/187028572-b963c1e1-e589-43ec-831e-69ef8b4db56b.png)

### 7) CircleCi
Added all files to the CircleCi and setup the project with the needed Environment variables
#### Checking CircleCi Environment list
![image](https://user-images.githubusercontent.com/77749264/187028392-104f4e75-be1c-4be5-993b-4c27ab0a20cb.png)
![image](https://user-images.githubusercontent.com/77749264/187028398-7551cea5-e3c9-4365-9191-b1ca430a141f.png)

#### Checking CircleCi Build
![image](https://user-images.githubusercontent.com/77749264/187028481-d526b9e0-ff1a-4268-aa2b-c9e7ea8fe325.png)

#### Checking CircleCi Deploy
![image](https://user-images.githubusercontent.com/77749264/187028508-cb4772be-4889-4075-99ba-3d6ed9df524e.png)

#### Last CircleCi Status
![image](https://user-images.githubusercontent.com/77749264/187028541-19dae0f8-48f4-438e-910b-004eb1890328.png)
