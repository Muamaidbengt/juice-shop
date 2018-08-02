# My setup of the Juice Shop for a CTF-style workshop

- I created the CTFd environment
  - I forked CTFd to my Github account (in the end, I didn't end up doing any changes to it here anyways)
  - I created a DockerHub repo and connected it to my forked CTFd Github repo (Continuous Build)
  - I created an Azure App Service and connected it to my DockerHub repo (Continuous Deployment)
- I created a "template" of the Juice Shop for workshop attendees
  - I forked Juice Shop to my Github account
  - I edited the Readme.md to simplify for workshop attendees
  - I edited the packages.json to enable CTF mode
  - I edited the ctf.yml to enable text hints (I left the default secret though, since I'm not concerned about cheating etc)
  - To test it, I created a Heroku app and connected it to my forked Juice Shop (Continuous Deployment)
- I configured the challenges etc in CTFd 
  - I ran the Juice Shop CTF CLI on my local dev box and created a zip file with the challenges
  - I imported the challenges into the CTFd app
  - I edited the CTFd start page and provided some brief instructions for the workshop attendees
