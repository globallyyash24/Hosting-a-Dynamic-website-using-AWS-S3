# Hosting-a-Dynamic-website-using-AWS-S3
# Unveiling the website using the AWS service and turning the ideas into Reality...!

~Go to the AWS management console and search for the S3 service in search bar.
![Screenshot (8)](https://github.com/user-attachments/assets/2d7abe1f-859c-4f41-ad3d-70f101302fa7)


~At there we'll get the S3 console and their click on create bucket.
![Screenshot (9)](https://github.com/user-attachments/assets/fdcb9fce-643d-4267-9244-71027a6616af)


~While creating the bucket make the bucket type as a general purpose and give the unique name to the bucket.
![Screenshot (10)](https://github.com/user-attachments/assets/6de9e26b-6a7c-452f-887a-4d778e70cd57)


~Make the ACLs enabled in the object ownership and other settings as it is.
![Screenshot (10)](https://github.com/user-attachments/assets/55557783-768b-4dc2-b445-025577894431)


~For the publically access of bucket, unselect the block all public access. So the bucket will be publically accessible.
![Screenshot (12)](https://github.com/user-attachments/assets/255d6160-6b6a-428a-9cf4-a6804c109e21)


~Scroll down and create the bucket.
![Screenshot (13)](https://github.com/user-attachments/assets/c3227de6-45b2-4f61-9051-4f1d569b29d2)


~The bucket is created.
![Screenshot (14)](https://github.com/user-attachments/assets/e6092a91-5992-478f-9c4c-836101e58822)


~Click on the bucket.
![Screenshot (15)](https://github.com/user-attachments/assets/47a38fa3-c395-4c37-9ce5-7f1a26582569)


~For upload the file, we have to create our html file. For that search for the notepad in our pc.
![Screenshot (16)](https://github.com/user-attachments/assets/423185f4-0e0f-46c9-aae5-fa971de5c0cc)


~Enter the data in the file and save the file as .html extension. As we are saving the file by the name of index.html
![Screenshot (17)](https://github.com/user-attachments/assets/ab05f817-9b83-45b3-b14b-552750b9938f)


~Now go the S3 service and upload this html file in our bucket.
![Screenshot (19)](https://github.com/user-attachments/assets/bd1e0b4f-961c-4edd-b86d-b1ebd016af8c)


~Go to the properties section of our aws-web-host01 bucket.
![Screenshot (20)](https://github.com/user-attachments/assets/debdd5c8-b8cd-45b8-8606-b37b572d7c1b)


~Scroll down and click on the edit of static website hosting.
![Screenshot (21)](https://github.com/user-attachments/assets/f3a8ce2c-4937-44c3-8a7a-bce70650da9e)


~Enable the static website hosting and then type index.html in the index document and save the changes.
![Screenshot (22)](https://github.com/user-attachments/assets/f7557546-8479-4e45-99a3-8bff11243ef7)


~Now go to the permissions of the bucket.
![Screenshot (23)](https://github.com/user-attachments/assets/17c4b828-0394-48ae-ad98-891913d085bb)


~Go to the edit bucket policy and create the policy generator and also copy the bucket ARN.
![Screenshot (25)](https://github.com/user-attachments/assets/42551659-d107-4164-a5c4-e08aec2819d3)


~In AWS policy generator,
~Select policy type as S3
~Give principal as "*"
~Select action as "Get Object"
~Paste the ARN number
![Screenshot (26)](https://github.com/user-attachments/assets/221018e0-9072-48e2-895f-cdf8aec2c82c)


~Click on add statement and then generate the policy.
![Screenshot (27)](https://github.com/user-attachments/assets/ce458ec5-a3e4-4ca0-b1c8-635ff3c7d4a6)


~Here is the policy with JSON document. Copy this file.
![Screenshot (28)](https://github.com/user-attachments/assets/784a5a96-547c-49a6-8e0b-c19b4fc5b950)


~Paste that file in policy section of edit bucket policy and make some change in the copied file. Add the "/*" at the end of resource. Here in our file, the resource is on the 11th line. It may be anywhere and depends on the file. After all this make the save changes.
![Screenshot (29)](https://github.com/user-attachments/assets/d3379401-e84f-4259-992c-1107a8ca5d21)


~Copy the URL of Bucket which is at the last of our bucket section.
![Screenshot (30)](https://github.com/user-attachments/assets/1bb010e7-78ba-4ea7-ad57-7e6040fa2e55)


~Go on the new browser and paste that copied link at there.
![Screenshot (31)](https://github.com/user-attachments/assets/3a4da336-cda7-4bb0-b6ec-34bca8a1b6b7)


~Our website is ready.....!
![Screenshot (32)](https://github.com/user-attachments/assets/ac2de40e-1551-4e1f-a299-a4a31a12b882)


# That's it.....We've Hosted a website using AWS S3.
# This is just beginning - let's innovate, collaborate and build the future together....!
