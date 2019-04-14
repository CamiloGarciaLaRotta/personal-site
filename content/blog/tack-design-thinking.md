---
title: "Tack Design Thinking"
date: 2019-04-13T11:16:28-04:00
tags: ["brainstorming"]
draft: false
story: false
---

The concept of a job application tracking helper came up for the semester project for ECSE 428 at McGill University.The purpose of the class is to apply learned SW Engineering methodologies and CS concepts to design and implement a product.  

Because groups were made of 15 students, the basic idea of a helper got expanded to accomodate extra features.We ended up with a web app (with auth & inhouse job applications) and a Chrome Extension helper.  

There was no rigorous process to understand the issue trying to be solved.
But I believe we did not hit so far from the target.
Hence, I want to go back to understanding the users, as well as framing the problems they encounter while job hunting.
I want to then strip down the existent system from any unecessary components, in order to have just a
standalone (no server required) browser extension which addresses some of the core problems of application tracking.

I take this opportunity to also put into practice a concept I was introduced to lately: [Design Thinking](https://static1.squarespace.com/static/57c6b79629687fde090a0fdd/t/5b19b2f2aa4a99e99b26b6bb/1528410876119/dschool_bootleg_deck_2018_final_sm+%282%29.pdf).  
This is by no means a discussion about its pros/cons. But rather a chance to use a tested approach 
to define a real problem and subsequently define an appropriate solution.

# Empathize (Observe, Engage, Immerse)

I find that written surveys are inefficient when it comes to empathize with users.
You loose the 1-on-1 conversation by hding behind a sheet of paper or an online form.
Asking at the end of the conversation questions such as: what do you think the problem is and what solutions you see for it
might give outside approaches (non-tech) which can prove very insightful. I also asked what would they call the application
because I had no idea what to call it.

## Interviews
### User #1
A grad student nurse working par time, heavy use of technology as service
- Her most common applications are not Job postings, but rather Scolarships/Bursaries.
  These applications require CV, transcripts andCover Letters (CL)
  Most applications have the same format
- In case she gets asked follow up information she needs to remember which documents she used
- Whenever she finds a posting of interest, she keepts a tab open with the URL.
  She uses session-buddy, a chrome extension that keeps bundles of tabs in memory.
  If she is on mobile, she will send herself a link through messenger
- She only applies via laptop. She feels unsafe filling forms on a mobile device.
  The CV, CL may be badly formatted but because of the screen size she wont notice.
- She suggests not calling the system XXXtracker, as it will give the impression that the system
  follows the application process giving updates on its status to the user.
- When asked about the solution she would propose she said a system which would sore locally a resume of 
  the application information (bursary name, cv used, date applied) in a file to be synched with her cloud

### User #2
Full time employee, political sciences grad, medium technology use

- He does not need multiple CVs nor CLs. He has a single one which he uses for each application
- He writes in his notebook reminders to apply for a given job.
- His field has mostly phone interviews. 
  He needs to remember quickly and find fast information he wrote about the position the moment he receives call. 
  Most of the time there is no notice of calling beforehand.
- Potentially not a user who might use heavily a technology solution

### User #3
Full time mechanical engineer, medium technology user

- He hasn't applied for jobs/scholarships in a while, but has been looking for a car lately
- He would take screenshots of the Kijiji post with the phone number and send it to himself over chat
- He would add comments to the message regarding questions he wanted to ask when he would meet with the seller. 
  Things too look out for the car's state. Price to propose
- Adding a field for comments might be useful

### User #4
Full time SW engineer, heavy mobile user

- He applies directly from mobile for any type of job posting
- He has a single CV, CL and has no need to keep track of multiple versions
- He writes questions to ask and things to remember about posts before the interview in Google Keep
- He has little need to save metadata of a given posting

### User #5
Full time cartographer, low technology use

- She is a low mobile user.
- She keeps a folder in her laptop with subdirectories for each job posting she applies to
  The subdirectories contain both files given via the posting (e.g. pdf of application) and
  files she submitted (e.g. CV/CL)
- She finds it ineficient to have to go through each subdirectory when she forgets the exact one she is looking for
  She has to sometimes sort by date created
- She would like an easy to search and easy to read indexing of her job applications
- If there were to be any application for this problem, she needs it to be a no-hussle access thing
  No need to go out of her way to open/login/setup/store info

## Personal Experience
Throughout my own job hunting process I have developped some approaches to manage my applications.
- when I find a posting of interest, I copy the URL and send it to my email. 
  I tend to do this with anything I want to do later: bookmarking an article, reminder to buy something, etc
- I have a master CV and many template CL. 
  For each application I tailor a CV & CL from the master versions.
  I notice that I tend to keep some specific versions of each of them. e.g. cloudCV, devopsCV, passionateCL, formalCL
- I never keep track of which specific CV/CL I used for each posting.
  I often have had to mentally try and remember what exactly I said to avoid mistakes during interviews.
  The worst situation came when I was contacted by phone by a company I had applied to and did not remember having done so.
  It gave a bad impression to the recruiter.
- After applying to many postings and being refused from many, I began wanting to plot my track as a way of coping.
  I manually wrote entries for each application with the status: 
  applied, interviewed, refused(company said no), declined(I said no), accepted.

# Define (express problems from POV of actors)

Bogdan, 21 y/o, part-time undergrad part-time employee, high tech proefficiency
actively applies for jobs
applies through both mobile and non-mobile devices

Eva, 25 y/o, graduate student, mid tech proefficiency
actively applies for scolarships & bursaries
never applies through mobile devicses

José, 32 y/o, full-time employee, mid tech proefficiency
ocassionaly applies for jobs
applies through both mobile and non-mobile devices

Debra, 55 y/o, full-time employee, low tech proefficiency
rarely applies for jobs
never applies through mobile devicses

Given the template: <user> is a <characteristics>, who needs <needs> because <insight>

Bogdan is a high technogy user currently working and studying at undergraduate level part-time,
who needs to remember which version of each CV CL he used for any application
because he wants to know what he might be questioned during the interview

Bogdan is a high technogy user currently working and studying at undergraduate level part-time,
who needs to visualize the status of his past applications
because he wants to know which CV/CL were most effective in getting him interviews

Eva is a mid technogy user currently in grad school,
who needs to remember deadlines for scolarship/bursary applications
because she wants to tailor the CL in advance

José is a mid technology user who has been in the workforce for over 5 years,
who needs to couple postings of interest with notes containing questions and comments
because he wants to remember key details whenever he meets with the person who published the posting

Debra is a low technology user who has been in the workforce for over 30 years,
who needs a simple access and search of job applications she has done
because she finds it inefficient to manually go through every folder in which she keeps the records


# Ideate (formulate key problem -> potential solutions)

An applicant needs to pair:
  - a posting
  - its deadline
  - its status (to apply/applied/denied/refused/accepted/interviewed)
  - comments about the posting (questions, things to remember)
  - the version of CVs/CLs (stored in desktop or cloud) to be used/used
in order to:
  - have time to prepare the CL
  - know what to prepare to be questioned in each interview
  - know which CVs CLs are the most efficient in landing interviews
  
An applicant does not want to have to go out of his way 
to perform the previous action,nor to search/view previous stored pairs


# Prototype
The comprimises I will make for the first iteration are:
  - not target mobile users. Only target destkop users
    the reasoning being that adding a mobile app to pair postings is of low interest for a person who
    is proefficient a submitting applications via the mobile. They would simply use their cloud app to
    retrieve & modify whatever documents they need
  - focus only on Chrome as its the most widely used web browser and has a rich API
  
As the original chrome extension was written in ReasonML + React, it is a potential candidate to build the first prototype.
The second option I see is using vanilla Javascript + React.
  
ReasonML:
PROS
  - solid type system
  - Optional Values
  - Pattern matching
  - Natively supported in React
  - Some of the code base is already available
CONS
  - API for promises and async is still a WIP
  - requires writing my own bindings for niche API's like Google Chrome Extensions
    Not necesarilly bad, as I would learn alot. But it would shift focus from developping a protorype to learning a new framework.
Javascript
PROS
  - up to date libraries and APIs
  - native language understood by the Chrome Extensions
  - fastes developping speed
CONS
  - need to write more tests to ensure appropiate input/output types
  - less confidence in my code
  - need to rewrite everything from scratch
    Not necesarilly a bad thing, I can review what was ugly in the oroginal extension and improve.

The first prototype I will develop will be in ReasonML, I will be able to reuse most of the existent code.
During the testing of this prototype I'll be able to measure the shortcomings of using ReasonML and its maintanability.
If to many bemols come up during the testing phase related to the code itself I will try a second prototype in Javascript.

# Test

# TODO
- pass MVP iteration plans from paper to Gist


