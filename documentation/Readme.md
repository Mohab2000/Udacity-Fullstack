### Creating database on aws

-Through aws console , navigating to RDS and then creating database. <br />
-After the creating, I set the policies to all traffics and IP to 0.0.0.0 so it's accessible. <br />
-Database end point: udagram-1.cojokxty5mbd.us-east-1.rds.amazonaws.com <br />

### Creating backend on elastic beanstalk

-Navigating to elastic beanstalk on aws and then creating the backend server. <br />
-After that I used the elastic beanstalk on the server by using eb use. <br />
-Last step is deploying our backend server to this elastic beanstalk environment. <br />

### Creating frontend on S3 Bucket

-Creating IAM user is needed for this step, so it's the first thing done. <br />
-Giving this user administrator access. <br />
-Navigating to S3 and then creating bucket. <br />
-After creating bucket is done, I had to set CORS and bucket's policies. <br />
-Bucket link: http://mohab-udagram.s3-website-us-east-1.amazonaws.com <br />

### Github and CIRCLE CI

-I pushed the code to my github account <br />
-Registered at CIRCLE CI and linked my account with github <br />
-Lastly, I could access all the projects in github through CIRCLE CI <br />
-CircleCI pipelines are the highest-level unit of work, encompassing a project's full . circleci/config. yml file <br />
-Setting all the scripts in circleci folder. <br />

### Why Circle CI?

-CircleCI allows the team to build automated pipelines and focus on real work innovation, I could automate for new commits it also reduces human error. <br />
-When developers commit and push changes, circle ci checks for changes made and track all of those changes. <br />

### Environment variables

-Setting environment variables was essential in (Elastic beanstalk - Circle CI - .env) <br />

### Environment variables used

```
POSTGRES_USERNAME= ""
POSTGRES_PASSWORD = ""
POSTGRES_HOST = ""
POSTGRES_DB = ""
AWS_BUCKET = ""
AWS_REGION = ""
AWS_PROFILE = ""
JWT_SECRET = ""
URL = ""
AWS_ACCESS_KEY_ID = "
AWS_SECRET_ACCESS_KEY = ""
PORT = 
DB_PORT=
RDS_DIALECT = ""
```
