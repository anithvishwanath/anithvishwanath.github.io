---
layout: post
title:  "cerTrax Training Module"
date:   2019-06-07 02:34:00 +1000
excerpt: Certification and training management system that keeps track of the personnel compliance and training requirements at mining sites.
categories: case-studies
---

cerTrax is a certification and training management system that keeps track of the personnel compliance and training requirements at mining sites. This falls in line with the Mine Safety and Health Administration (MSHA) guidelines which requires every employee is equipped with the proper training and certification standards set in place. 

In addition, MSHA also conducts routine inspections at mining worksites/areas. This may involve producing certification and training plans when requested. Having an application that both digitises and provides a way to manage personnel certification records along with their training programs undertaken will allow for greater portability and better competency at mines.

## The Ask

rapidBizApps needed a module (in addition to the certification management system already in place) for the web, that could also manage and keep track of personnel training. For example, cerTrax could be used to keep track of the training each employee has and also the equipment they are trained on. Furthermore, employees are awarded a certificate at the end of their respective courses.

### Goal

> Help the mining industry develop high-quality training programs as part of MSHA’s mission to keep miners safe and healthy.

### Understanding the problem

I began by going through the current implementation of the system to better understand the problem. A contextual inquiry was required but it was obviously not possible to perform a field study remotely. All of the requirements gathering was made possible by studying the training plans and the guidelines outlined by MSHA, and also by asking questions to the stakeholders. This resulted in a relatively low chance of working based on assumptions. 

The application was scoped out to have three main user groups -- an administrator, a supervisor, and the operator. The app will have a set of capabilities assigned to each role. During my research, I found that some mine operators can provide training to other operators. In other words, certain mine operators may also provide training (on the condition that they have been authorised to impart their knowledge in their area(s) of mining operations expertise by MSHA). These operators are referred to as “Competent Persons” within the MSHA program policy manuals, however they are simply called “Trainers” within the context of our application. Trainers here may either be in-house personnel, or external consultants (independent contractors). Training can also be conducted either on-site (work areas owned by the mining company using the application), or off-site (external locations; supervisors elect to send a cohort of miners for training purposes).

I started out by making the application solely for a mine supervisor. 

#### On training plans

All training plans developed by mine operators and/or independent contractors must be approved by MSHA and must be made available upon request. A training plan contains information related to the teaching methods, course materials, evaluation procedures, and the estimated teaching time for each subject. A training plan is automatically considered approved by MSHA if it contains all the requisite data. If a plan does not include the required information, it must be subimtted to the appropriate MSHA regional manager for approval; mine operators are notified in case the plans are not approved (in which case they may appeal the decision).

The application would therefore have to provide a way to allow the user to formulate a training plan and also to capture all the data, which must be subject to approval. The module was thus going to have three core functions: 
* Add/create new training plan, which must then be approved
* Schedule an approved training plan
* Add personnel to the training plan

### User flow map

I made a user flow model with a set of functions that maps the supervisors' tasks through the functions present in the training module.

![User flow diagram for the training module](/images/ct/user-flow.png)

A higher-res version of the flow diagram can be viewed <a href="https://www.anithvishwanath.com/images/ct/user-flow.png" target="_blank">here</a>.

## Ideation

For the design, I first started by sketching the concept on paper. A way to capture the training plan data was via simple forms on the web. I however had to figure out a way to show the main training view, as training plans had statuses assigned to them (active / pending approval / unscheduled). Moreover, the training plans must also indicate the overall progress of each course -- which is tied to the course duration (for the supervisor view).

### Prototype

The interface design began by referring to the initial sketches I made along with the requirements gathered by perusing the MSHA training plan guides, specifications, and referring to sample training plans (for the forms). I initially made a set of wireframes, which gave me ample opportunities to iterate. Select screens are shown below.

#### Training plan view

The interface was going to make use of the existing layout and structure, with certain new elements added to it. Primarily, I wanted to establish a clearer visual hierarchy via better typography and colour. Secondarily, I felt the need to simplify the interaction points. The training plan view shown below was made to meet both these needs. I chose blue for the primary elements of the interface. 

![Training plan view](/images/ct/training_view1x.png)

For example, the blue header for the cards in the screen above indicates active training plans. These plans also have a progress bar tracking the course progression. Similar colours have been chosen to indicate different states; grey for unscheduled training plans, and yellow for those pending approval. This is a deliberate design decision, instead of being more explicit via the use of labels / tags, which have been repurposed to show the teaching methods used for the courses (as seen in the active training module section below).

#### Active training plan details

![Active training plan view](/images/ct/active_training_module1x.png)

The layout for the active training plan was designed to ensure each element has proper form and definition. All elements are given equal emphasis via the use of cards. This allows for easy visual scanning and less cognitive load; information can be gathered at a glance. The active plan shows the teaching methods used (lectures / discussions), the subjects included (which can be expanded to show more details), the evaluation procedures, and the training materials (for use by trainees). An overview of the course, along with the personnel information is shown on the right-hand side. One particular challenge I faced was to make optimum use of the screen space available on the web; the data had to be divided into different groupings and placed in a way that can be accessed effortlessly. 

#### Creating and scheduling training plans

Creation and scheduling of training plans is done through forms. Both forms have been divided into logical groupings, with appropriate description for each.

![Create new training plan](/images/ct/new_plan1x.png)

The forms have been designed in line with the MSHA training plan development specifications. Training plans can be scheduled both on- and off-sites. When off-site locations are selected, an address field is shown. Supervisors can also assign a trainer and a set of trainees to the plan that they select to schedule.

![Schedule training plan](/images/ct/schedule_plan1x.png)

Thank you for reading!
