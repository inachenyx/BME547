# BME 547 - Medical Software Design - Fall 2021  

## Instructor
Dr. David Ward  
<david.a.ward@duke.edu>  
Office Hours: By appointment

## Teaching Assistants
Lillian Ekem  
<lillian.eken@duke.edu>   
Office Hours: By appointment

Yuan Tian  
<yuan.tian277@duke.edu>  
Office Hours: By appointment


## Course Delivery
### Lecture
Monday / Wednesday 12:00 pm to 1:15 pm  
Location:  Wilkinson 126

Attendance at lectures is an expectation of the course.  
Bringing a laptop computer for working in class is highly recommended.

### Safety Protocols
Following Duke-mandated safety protocols is required for this class and
students who fail to follow these protocols will be asked to leave the 
classroom until they can comply.  The most recent Duke protocols can be found
at <https://coronavirus.duke.edu/> and <https://returnto.duke.edu/>.

### Pre-lecture videos
Some content will be delivered via pre-recorded videos that should be
watched before class, with an accompanying quiz to check for understanding.
Please see the "Attendance / Participation" section below for more information.

### Official course communication
Sakai will be used for official course communication.  

### Assignments
A variety of projects will be assigned throughout the semester.  The 
description of these assignments will be posted in Sakai and also in this 
GitHub repo.  Assignments will be turned in via a GitHub Classroom repository.
Assignment feedback will be delivered via Gradescope and Sakai.

## Course Overview
Software plays a critical role in almost all medical devices, spanning device
control, feedback and algorithmic processing.  This course focuses on software
design skills that are ubiquitous in the medical device industry, including
software version control, unit testing, fault tolerance, continuous integration
testing and documentation.  Experience will be gained in the Python programming
language.

The course will be structured around various software projects related to
medical devices and databases that measure and process biosignals, send 
information to a web server, and makes those data accessible to a web client.
The projects will be designed to develop software
design fundamentals.   Some project-related work will be done in groups.

## Prerequisites
Basic familiarity with programming concepts (e.g., variables, loops,
conditional statements, functions and parameters).

BME 271 - Signals and Systems

A computer with administrator rights and good internet connection.

Complete the prerequisite assessment found 
[here](Assignments/00_programming_assessment.md).

## Course Topics
* Software version control (`git`, GitHub)
* Device programming fundamentals
  + Review of data types, variables, loops, conditional statements
  + Python (v3)
  + Use of external libraries / packages
  + Virtual environments & dependency management (`pip`, `requirements.txt`)
  + Use of a programming IDE
  + Debugging (`pudb`)
* Testing
  + Unit testing
  + Functional / System testing
  + Continuous integration (GitHub Actions)
* Fault tolerance (handling and raising exceptions)
* Logging
* Documentation
  + Docstrings
  + Markdown
  + Sphinx
  + [ReadTheDocs](https://readthedocs.org)
* Working with data
  + Data Storage (Text, Binary, MongoDB)
* Data Processing & Display
  + Jupyter Notebooks
  + Matplotlib
  + Numpy
  + [scikit-image](https://scikit-image.org/) & [scikit-learn](http://scikit-learn.org/stable/)
* Servers
  + Design & Implementation of a biomedical web service (Python Flask)
  + HTTP & RESTful APIs
* Medical Software Development Standards

## Attendance / Participation
Lecture attendance and participation is important as the topics and skills you
will be learning build upon each other.  Also, you will be working
in small groups some of the semester.  Various "daily assignments" will also 
be given as part of either class period preparation or during the class 
period itself.  

If a class member cannot join the class period for any reason, they must
contact the instructor ahead of time to make arrangements.  It would then be
expected that this person will view the lecture recording and
complete any given daily assignment before the next scheduled class meeting.

Before some lectures, a pre-recorded video may be assigned for viewing with
an accompanying quiz.  Watching the video and completion of the quiz is 
expected to be done before the class period begins.  

Attendance in class, watching pre-class videos, completing pre-class quizzes
on time, and completion of assigned in-class activities 
will count for 15\% of your class grade.  Eighty percent successful completion
of these activities is required to earn the entire 15\%.  Participation points
will be decreased for completion rates less than 80\%.  

It is very understandable
that students will have to miss class for job interviews, personal reasons,
illness, etc.  Absences or delayed daily work will be considered **excused** 
if they are communicated to and approved by your instructors at least 48 hours 
in advance (subject to instructor discretion as an excused absence) or, 
for illness, through
submission of a [Short Term Illness Form
(STIF)](http://www.pratt.duke.edu/undergrad/policies/3531) **before** class.
Unexcused absences will count against the participation component of your class
grade.

## Textbooks & Resources
There are no required textbooks for this class.  A variety of online resources
will be referenced throughout the semester.  

* [Python Resources](Resources/python.md)

## Project Details
Project details will be discussed in lecture throughout the semester.

## Grading
Official assignment posting will be done in Sakai.  The detailed assignment
description will be done in this GitHub repository.  Assignments will generally
be submitted in a GitHub Classroom repository.

Due dates--including those that change--will be announced in lecture and by
Sakai announcements that will be emailed to the
class.  
<table>
<tr>
<th>Grading Breakdown</th><th></th>
</tr>
<tr>
<td>Participation / In-Class Assignments / Pre-Class Quizzes</td>
<td>15%</td>
</tr>
<tr>
<td>Assignments</td>
<td>45%</td>
</tr>
<tr>
<td>Final project</td>
<td>40%</td>
</tr>
</table>

All work is due by the date and time posted in Sakai.  No late submissions will
be accepted without prior written approval for an excused reason.  You will
be given the opportunity to submit *one* assignment (not including the Final
Project) up to 48 hours late 
for any reason without penalty if you notify me that you are utilizing that
option before the deadline via e-mail.

Specific project feedback will be given using Gradescope and Sakai.

## Class Schedule
The course schedule is likely to change depending on progress throughout
the semester.  The [schedule](schedule.md) will always be available in
the GitHub course repository, but is always subject to change.  Assume there 
will be a lecture every class period even if no topic is shown on the schedule.

## Distributed Version Control Software (git)
Software management is a ubiquitous tool in any engineering project, and this
task becomes increasingly difficult during group development. Version control
software has many benefits and uses in software development, including
preservation of versions during the development process, the ability for
multiple contributors and reviewers on a project, the ability to tag
*Releases* of code, and the ability to branch code into different functional
branches.  We will be using [GitHub](https://github.com) to centrally host our
git repositories.  Some guidelines for using your git repositories:

* *All* software additions, modifications, bug-fixes, etc. need to be done in
  your repository.
* The *Issues* feature of your repository should be used as a "to do" list of
  software-related items, including feature enhancements, and bugs that are
  discovered.
* There are several repository management models that we will review in class,
  including branch-development models that need to be used throughout the
  semester.
* Instructors and teaching assistants will only review code that is committed
  to your repository (no emailed code!).
* All the commits associated with your repository are logged with your name
  and a timestamp, and these cannot be modified.  Use descriptive commit
  messages so that your group members, instructors, and teaching assistants can
  figure out what you have done!!  You should not need to email group members
  when you have performed a commit; your commit message(s) should speak for
  themselves.
* Code milestones should be properly tagged.
* Write software testing routines early in the development process so that
  anyone in your group or an outsider reviewing your code can be convinced that
  it is working as intended.
* Modular, modular, modular.
* Document!
* Make commits small and logical; do them often!

We will review working with git repositories in lecture, and feedback on your
software repository will be provided on a regular basis.

## Duke Community Standard & Academic Honor
Engineering is inherently a collaborative field, and in this class, you are
encouraged to discuss what you have learned in class and share resources that
you find.  However, your code development and final submitted code must be the 
product of your and/or your assigned group's effort and understanding.  It is not 
permitted to share your code with others for them to review, copy, or use.  Any 
freely-available, external 
resources developed by others, and used in your project,
must be properly recognized.  These outside resources must be clearly published
for general use and cannot be the work of other current or former Duke students.

In general, if you can install it from a package manager, such as `pip` or 
`conda`, then you can use it as part of your work.  If you cannot, you should
seek further guidance from the instructor.

All students are expected to adhere to all principles of the [Duke Community
Standard](http://www.integrity.duke.edu/standard.html).  Violations of the Duke
Community Standard will be referred immediately to the Office of Student
Conduct or the appropriate Graduate School dean.  Please do not hesitate to 
talk with your instructor about any situations involving academic honor, 
especially if it is ambiguous about what should
be done.  More information on the Duke Community Standard, and its practice
for this academic year, can be found at 
<https://registrar.duke.edu/university-bulletins/duke-community-standard>.

For undergraduates, if a student is found responsible through the Office of 
Student Conduct for
academic dishonesty on a graded item in this course, the student will 
receive a zero for that assignment, and the final grade for the course will be
reduced by at least one full letter grade.  If a student's admitted academic
dishonesty is resolved directly through a faculty-student resolution agreement
approved by the Office of Student Conduct, the terms of that agreement will
dictate the grading response to the assignment at issue.

For graduate students, the appropriate policies of their graduate school will 
apply.  
