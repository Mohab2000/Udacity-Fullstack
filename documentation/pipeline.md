### Creating database on aws

-Through aws console , navigating to RDS and then creating database.
-After the creating, I set the policies to all traffics and IP to 0.0.0.0 so it's accessible.
-Database end point: udagram-1.cojokxty5mbd.us-east-1.rds.amazonaws.com

### Creating backend on elastic beanstalk

-Navigating to elastic beanstalk on aws and then creating the backend server.
-After that I used the elastic beanstalk on the server by using eb use.
-Last step is deploying our backend server to this elastic beanstalk environment.

### Creating frontend on S3 Bucket

-Creating IAM user is needed for this step, so it's the first thing done.
-Giving this user administrator access.
-Navigating to S3 and then creating bucket.
-After creating bucket is done, I had to set CORS and bucket's policies.
-Bucket link: http://mohab-udagram.s3-website-us-east-1.amazonaws.com

### Github and CIRCLE CI

-I pushed the code to my github account
-Registered at CIRCLE CI and linked my account with github
-Lastly, I could access all the projects in github through CIRCLE CI
-CircleCI pipelines are the highest-level unit of work, encompassing a project's full . circleci/config. yml file
-Setting all the scripts in circleci folder.

### Why Circle CI?

-CircleCI allows the team to build automated pipelines and focus on real work innovation, I could automate for new commits it also reduces human error.
-When developers commit and push changes, circle ci checks for changes made and track all of those changes.

### Environment variables

-Setting environment variables was essential in (Elastic beanstalk - Circle CI - .env)

### Environment variables used

```
POSTGRES_USERNAME= "postgres"
POSTGRES_PASSWORD = "postgres"
POSTGRES_HOST = "udagram-1.cojokxty5mbd.us-east-1.rds.amazonaws.com"
POSTGRES_DB = "postgres"
AWS_BUCKET = "arn:aws:s3:::mohab-udagram"
AWS_REGION = "us-east-1"
AWS_PROFILE = "default"
JWT_SECRET = "mysecretstring"
URL = "http://udagram-1.cojokxty5mbd.us-east-1.rds.amazonaws.com"
AWS_ACCESS_KEY_ID = "AKIA4J3FLUA7KNPIV3GU"
AWS_SECRET_ACCESS_KEY = "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"
PORT = 8080
DB_PORT=5432
RDS_DIALECT = "postgres"
```
