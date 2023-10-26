## Security Module
 Welcome to the Security Module of ProductLab. We've scaled pretty rapidly over the past four modules. Now you should understand how to build a basic fullstack web application (some of you may have even built your own last module!). You also should have an awareness of the complexities that arise in more sophisticated systems. But our clients need solutions that don't just work efficiently, but work securely. Cybersecurity is a constantly evolving field. Don't take this module and assume you're "done." Instead treat this as your orientation!

 ## Housekeeping
 Please watch this repo by selecting the "watch" button, which is directly above the bright green "Code" button. This will help us keep track of participation.

 To keep a central record of your accomplishments you will need to create a repository called 'Security_yourname' and then upload each project to the repository. This will allow your instructors to easily review your work! Your final project will also link to this repo to demonstrate your Security skillsets. 

 This repo will serve as both your solution files as well as the rubric for how you should name and structure your files. 

 ## Assignments: Academic 
 Before working on the hands on material please review the following: 

1. [An introduction to security protocols and types of attacks](https://www.bitdefender.com/cyberpedia/types-of-security-protocols/)
    * This article throws you in pretty quick, take your time with it. Don't skip the video at the beginning of the article, it will help give context to what you read and (hopefully) make it easier to understand. 
    * Also remember your previous Modules, we have covered the different layers of the internet (physical, data link, network, etc) if you've forgotten check out this [quick article](https://www.networkworld.com/article/3239677/the-osi-model-explained-and-how-to-easily-remember-its-7-layers.html)

2. [Now, what is OAuth 2.0?](https://auth0.com/intro-to-iam/what-is-oauth-2) 
    * OAuth is a very useful tool you will almost certainly run into on one of your engagements. This article is a quick intro. 
        * If you want to be extremely overwhelmed you can look through [this documentation](https://oauth.net/2/) but frankly I wouldn't. It gets extremely technical very quickly
    * Its important before we go farther to understand the difference between authorization and authentication. [read this](https://www.geeksforgeeks.org/difference-between-authentication-and-authorization/)
        * This may seem like an unneeded distinction, but to communicate with technical stakeholders you have to understand this distinction
    * Finally, lets look at OpenID, an authentication protocol. [read this](https://www.pingidentity.com/en/resources/identity-fundamentals/authentication-authorization-standards/openid-connect.html)

3. [Public Key Infrastructure](https://www.youtube.com/watch?v=0ctat6RBrFo)
    * This is your crash course in cryptography. To quote Fast Times at Ridgemont High: "Learn it. Know it. Live it."

4. [JSON Web Tokens aka JWTs](https://jwt.io/introduction)
    * The above is an introduction to JWTs, [read this article](https://fusionauth.io/articles/tokens/pros-and-cons-of-jwts) to get a better idea of the pros and cons.
    * if you're looking for a different explanation, check out [this youtube video](https://www.youtube.com/watch?v=7ozQLeFJpqs) for a quick 2 minute summary of JWTs!

5. The next two videos will cover hashing and sharding. It feels very mathy but stick with us. Its not just something developers need to worry about. As a Product Manager hashing and sharding are concepts you'll absolutely be expected to understand.
    * [An introduction to Hashing and Security](https://www.youtube.com/watch?v=b4b8ktEV4Bg)
    * [An introduction to sharding](https://www.youtube.com/watch?v=be6PLMKKSto)


## Assignments: Hands On
Enough reading! Time to make some stuff! 
1. Create a new repository in your Github called "Security_yourname"
    * This is where you will store your work for the module. 
    * Make sure the repo is "public"
        * go to settings, scroll down to the "Danger Zone" section and change the repo to public

2. Navigate to [this hash generator website](https://www.md5hashgenerator.com/)
    * Type in a sentence and then generate the hash. Now make a small change to your sentence and generate a new hash. Play around with this and see how even extremely small changes can have huge impacts on the hash! 
    * Take a screenshot of your sentence and the resulting hash and upload it to your github repo. 

3. Now, we'll do a similar exercise but with JWTs. Navigate to [this JWT generator](https://jwt.io/)
    * Don't mess with the header, you'll get an error if you change that part
    * Leverage what you learned in the API module with JSON structure. Update the payload section however you would like. Again see how small changes can have big impacts ont he encoded token. 
    * Take a screenshot of your updated payload and token and upload it to your github repo.
    * Also, click "share JWT" then paste it your into the ProductLab general chat along with your secret key so other people can 'decrypt' your token and authorize their signature! 
        * I'll go first: https://jwt.io/#debugger-io?token=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJQcmFjdGljZSI6IkRFVCIsIm5hbWUiOiJQcm9kbGFiQWRtaW4iLCJmYXYgZm9vZCI6ImNoaWNrZW4gcGFybSIsImxvY2F0aW9uIjoiU2FuIEZyYW5jaXNjbyIsImlhdCI6MTUxNjIzOTAyMn0.fqJ1Z9dj4cZ9kVwhieOVHqAPGvWHRSzQBYrcPwQ3Be0
            * Signature: productlabRULES!
    * NOTE: please don't put any actual sensitive information in this JWT exercise 

4. Finally, its time to implement some security into an API. You have built RESTful APIs before, this time you'll follow a similar project but implement AuthO as a security measure. 
    * follow the tutorial [here](https://auth0.com/blog/node-js-and-express-tutorial-building-and-securing-restful-apis/)
    * Note: this tutorial shows 'insomnia' screenshots, ignore that and just use Postman
    * upload the file tree of the API you built j
    * and upload a screenshot of Postman hitting your secure endpoint

## Assignment Format 
At the end of the week we expect your Github repo to have the following files: 

1. A screenshot of your hashing experiment
2. A screenshot of your JWT experiment
2. the entire file structure of your secure API project
3. a screenshot of Postman hitting your secure endpoint

## Troubleshooting

If you have any trouble navigating the GitHub repo or working on the exercises, please don't hesitate to ask for help. The Admin Team and your Instructors are always happy to help.