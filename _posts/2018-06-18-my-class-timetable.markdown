---
layout: post
title:  "My Class Timetable"
date:   2018-06-18 12:34:09 +1000
excerpt: Swinburne University timetable application redesign.
categories: case-studies
---

![My Class Timetable](/images/mct/f_header.png)

My Class Timetable is an online timetable management module used by students, faculty, and the administrative staff at Swinburne University of Technology. It is part of a student management system called Student One, developed by Swinburne. Users may register, swap or change their classes upon the commencement of a semester using the application.

<!--more-->

The following report is a concrete case study of My Class Timetable along with a solution to the problem space I have done when I was a student studying the User-Centred Design unit at Swinburne. I was part of a group that worked on the project which took 3 months to finish, incorporating all the design principles and practices taught to us during the course.

## Context of use

I began the process by first defining the goal and understanding how users operate the system in different environments.

### Goal

> Redesign My Class Timetable so that it adheres to the user-centred design principles and practices, ultimately offering a good experience.

I observed that the application is designed to be used at homes/offices on computers. Users may interact with each other by means of sharing or exporting their timetables. I then started analysing the current user interface, and scoping out prospective user groups. The application is exclusive to users belonging to Swinburne in any capacity – either students or staff – and as such, only they have access to the timetable. They serve as our user groups in this context. The tasks both user groups perform are functionally similar in that they can register, update, view, and export their timetables. I focused on enhancing the app for the students user group.

![Current application interface (My Class Timetable) as viewed in a web browser](/images/mct/null1.png)

During the contextual inquiry, my colleagues and I identified common design problems listed as follows:

### Pain points

The time blocks for different classes are not rendered properly within the confines of the application grid. In some cases, the blocks render outside the confines of the grid / table.The time blocks for different classes are not rendered properly within the confines of the application grid. In some cases, the blocks render outside the confines of the grid / table.

* **Unclear unit names:** Unit codes are shown instead of the full name, which may be confusing to new students unfamiliar with unit codes.
* **Inability to change individual classes:** Users enrolled in two different classes in a unit, say a lecture and a tutorial, cannot change any of the individual classes. While swapping, they see both the lecture and the tutorial classes, when instead they may simply want to change their lecture to a different time slot.
* **Lack of support for mobile screens:** The application is not responsive thus lacking portability, which might be critical to a student wanting to see their next class – especially in a hurry.
* **Layout issues:** The time blocks for different classes are not rendered properly within the confines of the application grid. In some cases, the blocks render outside the confines of the grid / table.
  
  * The timetable layout breaks when the user adjusts the timetable size (done by dragging one of the ends of the grid of the timetable).

After the analysis of the current system and obtaining a rough idea about the context of use, I decided to have a brief conversation with fellow students and colleagues at Swinburne about the state of the application by recording their opinions, which led to

### Conducting user interviews

The interview process began with me preparing a list of open-ended questions. We were taught during the course to follow proper ethical procedures since the research involved studying user activity. I gave each participant a quick brief and also made sure that their anonymity was preserved. The participants were rewarded for their time, and were also given the right to withdraw from the study any time they wanted.

#### Material

I prepared the following list of open-ended questions for the interview:

* What is your experience with My Class Timetable like?
* How long have you been using it for?
* Did you register for all of your classes by yourself for this semester?
   * If you did, were you happy with your class selection?
   * If not, did the system do a good job choosing your schedule for you?
* Have you ever swapped/changed your classes (or considered)?
* Were you able to swap your classes easily?
* Did you end up swapping your classes?
* Do you use My Class Timetable on any other devices?

Standard note keeping equipment was used to record the interview data; pen and paper. All interviews were conducted on campus. I interviewed three students – each studying different courses. The recruitment took place on the university campus grounds with duly acknowledged informed consent.

The full interview transcript can be read <a href="https://docs.google.com/document/d/1YOnUL4x1lqicN66mMN2mgFHfJDA6aTh8qdlz0fUnkeI/edit" target="_blank">here</a>.

## Data Analysis

With the data gathered from the interviews, I set about analysing the data qualitatively. This involved building various models to represent the requirements gathered from the contextual inquiry.

### Affinity diagram

First, I created an affinity diagram based on the synthesis of the data from the contextual inquiry. Three major themes were identified from the synthesised data; represented in the form of blue-bordered boxes in the figure below. Relevant notes are shown under each theme. The affinity diagram may be viewed <a href="http://popplet.com/app/#/3087956" target="_blank">here</a> (requires Flash), or <a href="https://trello.com/b/fDK100ps/affinity-diagram" target="_blank">here</a>.

![Affinity diagram (card sorting)](/images/mct/null2.png)

I then created a user persona to better fit the population with the behavioural patterns, goals/motivations, and pain points.

![MCT Persona; Sally Brown](/images/mct/mctpersona.png)

The persona helped me understand the needs of an average university student using My Class Timetable for their timetable/scheduling needs. It justified certain elements within the app highlighting certain areas of difficulty experienced when changing classes, and also not being able to clearly see the class timings along with the respective locations.

### Competitive analysis

During my research, I was also looking into the timetable applications used by other educational institutions in Australia to both analyse and gain some insight and inspiration. This proved to be tough mainly because I did not have access to the student timetables as I was not enrolled into these institutions, nor did I know anybody attending them.

However, I managed to find some user guides that provided me enough data to piece together the features.

| Features      | Swinburne (My Class Timetable) | RMIT (myTimetable) | UNSW (Class Timetable) | Monash (Allocate+) |
| ------------- | ------------------------------ | ------------------ | ---------------------- | ------------------ |
| **Automatic Registration into classes** | Yes – clicking on the “Register into clash-free classes” button | No | Yes – clicking on the “Auto Timetable” button | Yes – the system automatically allocates classes if there is only one session |
| **Preferential class allocation** | No – students may have to contact the administrative staff at StudentHQ | Yes – students can indicate their preferred classes for certain courses for a short period of time | No | Yes – students can indicate their preferences for certain courses for a short period of time |
| **View timetable by week** | Yes – choosing a week in the current teaching period and clicking “Refresh” | Yes, although can see only the current week and all weeks | Yes – ability to see classes per specific weeks in a teaching period | Yes – can see classes for the current week and for all weeks |
| **View timetable by semester or the teaching period** | Yes – selecting the unit and clicking “Refresh” | Yes – via the “Search” button on the left sidebar | Yes – clicking on “Class Search” and choosing a teaching period | Yes – via the “Search” button on the left sidebar |
| **View timetable by day / month** | No | Yes – filtering possible | No | Yes – filtering possible |
| **Download / export / share timetable** | No | 	Yes – clicking on the download icon next to the print button | No | Yes – clicking on the download icon next to the print button |
| **List / grid view** | No – the default view is a grid | Yes – both list and grid views are possible | No – the default view is a grid | Yes – both list and grid views possible |

Through my analysis, I found both RMIT and Monash using the same vendor system for timetable management (Allocate+). It is also apparent that most of the applications have a common functionality, and there are some missing features in Swinburne’s My Class Timetable.

### User flow

I developed a user flow model with a set of predetermined tasks aiming to map the steps a user takes to perform certain tasks in the timetable. The user flow below shows a high-level view of the system and the tasks a user is expected to perform.

A high-res version of the user flow below can be viewed <a href="https://dl.dropboxusercontent.com/s/06duak839m6ecb0/mct_userflow.png" target="_blank">here</a>.

![User flow diagram](/images/mct/mct_userflow.png)

The user flow diagram helped me give priority to certain features. With all the requirements collected, it was time for

## Conceptualising the Design

I started by sketching out the concept in my sketchbook, which served as an entry point for my ideas. It had a potential to generate an influx of ideas because of my stream of consciousness technique in that I allow thoughts and ideas to come to me as I work. However, I kept things in check by referring back to the information architecture and the user flow.

![Conceptual sketches](/images/mct/mct_concept_sketch.jpg)

### Reintroducing My Class Timetable

I translated my initial concept art to a series of (fairly) low-fidelity prototype using Balsamiq mockups. I started with a mobile app mockup because it was the focal point of discussion in the user interviews – users wanted to see a mobile version of MCT. Also of note, I discovered Swinburne already has an official app, which has a module for My Class Timetable. Although, tapping the module simply takes the user to the timetable website, which is not supported on mobile devices and is hence not desirable. I decided to incorporate My Class Timetable as an actual component in the app that enables users to add, view, and update classes as per their enrolment.

The main challenge for me at this stage was figuring out the implementation of a grid-like calendar view for mobile devices, as tables and/or grids translate badly to mobile devices. After some research, I solved the problem by deciding to make the header parts of the table static, so the user would only have to scroll within the data portion, effectively seeing their classes corresponding to a particular day/time.

The full set of wireframes may be viewed (and interacted with) <a href="https://balsamiq.cloud/syg0c2s/pkvrd68" target="_blank">here</a>.

#### User onboarding

The app requires a user to authenticate using their student ID and password. Once authenticated, they have the option to view or update schedule for their enrolled units.

![Onboarding — dashboard view, expanded unit list when activated](/images/mct/1_registration.png)

Corresponding activities are shown when the user taps on a unit in the list. The activities clearly have a state assigned to them indicating the registration status. The states are accomplished with the help of clear and simple icons placed relative to each activity.

#### Unit registration and swapping

Selecting an activity directs the user to the registration screen, if they are a first-time user. Users are shown a list of all the available classes in the current teaching period, and can view more details and register into a class by tapping on an availability.

![Registration process for a lecture including information pertaining to an availability](/images/mct/2_registration-process.png)

Clicking on an availability takes the user to a screen which contains additional details of the associated activity. As seen in the figure above, the user is shown a map and/or a picture of the campus building where the activity is going to take place, along with details regarding the class location, a short summary that outlines the instructors’ names and the start and the end dates. Lastly, the user may click the register button if they wish to register into the chosen availability.

![Successful registration for an activity (lecture)](/images/mct/2_5_reg_lec.png)

In some cases, when there are no classes available for the user to register, the class is shown as a disabled state. Consequently, the user will have the option to see the class, but are waitlisted if they decide to register into the timeslot. They are automatically allotted the class once other users swap or if the administration decides to allocate additional slots for students.

![Disabled state for classes that do not have additional slots available (in this case, Fridays); waitlisting imminent](/images/mct/3_waitlisting.png)

Once a user registers into all activities, they may swap into another class – provided there are additional classes. The swap module is functionally similar to the registration module in that the user has the option to choose an availability to swap to.

![Class swapping (for a lecture)](/images/mct/4_unit-swapping.png)

Once all classes have been registered successfully, the user will have the option to further modify their class scheduling, or may view their timetable.

![Successful scheduling for an enrolled unit](/images/mct/4_5_final-classes.png)

#### Optimising the timetable view

The user has the option to see both a weekly (grid) view and a daily (list) rundown of their schedule in the app. This stage proved to be a significant challenge for me and I spent the most time researching how I might effectively show a grid/weekly view of the timetable on small viewports.

![Timetable view — Weekly view (on the left), and daily view (on the right)](/images/mct/5_timetableview.png)

Units are colour-coded, so each unit will have a unique colour assigned to it. The timetable for the grid has a fixed header for the days and the time so only the table data is scrollable.

A live version of the all the screens for the app can be viewed <a href="https://www.figma.com/file/0Www5kckwcS227eznSwNcNNU/My-Class-Timetable" target="_blank">here</a>.

## Wrapping Up

When I originally worked on the project as part of my academic curriculum, one of the final stages of the project for my group was to perform a usability test in a lab conducive to testing. The laboratory had different tools and equipment that we could use to record participants and observe their behaviour. Since I have graduated, testing the timetable in a relevant contextual setting will be tough.

I have thus far designed the interface that conforms to my flow models. However, there remain some additional questions that need answers. To this end, I have posited a list of assumptions that serves as a summary and may also warrant further analysis.

* Most students would love to have a mobile version of their timetables. The university has an official app that has a timetable component but it currently simply redirects the user to the web version on their mobile devices.
* Students will be willing to place some time and effort to get the timetables scheduled the way they want.
   * That said, not all students will be technically savvy or will have access to technology. Also applicable to users not using smartphones or applications.
* Most students manually enter their class schedules into the calendars native to their mobile devices.
* As a corollary, could the app use a native calendar, instead of a whole new calendar developed specific for the app? (a.k.a. reinventing the wheel)
   For example, Google calendar could be used for Android phones, and its iOS counterpart for Apple devices. (Since the export module on the web version will be producing files that support native calendars for phones anyway).

This project is a revisionism of a previous iteration that I worked on with my group. I actually decided to go with a fresh take, with some data from my contextual inquiry (for instance, the observation points and the student interviews) researched previously. Everything else (the models, concepts, and designs) is new because I have been constantly learning so much and have dedicated all my time towards user experience design as I find it very fascinating.

Thanks for reading!
