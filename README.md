# s3_password_authentication_bucket

1)Firstly create a demo website from Below Link
    https://www.free-css.com/free-css-templates

2)Select any image  and click on it. Now Download Option will appear Click on it.
![images/download.png]

3)Now extract the file and upload the content to S3 Bucket
![images/s3.png]

4)Now create a CDN using Amazon console.

![images/cloudfront_distribution.png]

5)Now create a lambda function from scratch using nodejs with Permission as Below
![images/lamdba_role.png]

6)Now go to CDN click on CDN NAME and click on Behaviour
![images/behaviour.png]

7)Now click on edit in Behaviour Section and you will find the option Function associations.Select Viewer request  select function type as LAMBDA@EDGE & FUNCTION ARN/NAME  of Lambda function (arn:aws:lambda:us-east-1:911126966751:function:lamdba_function_password_protected:2)

![images/lamdba_cdn.png]

8)Click on Save option. And you will find the CDN working as per you requirement.