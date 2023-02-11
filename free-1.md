# Free project 1

## The user and a language

This section describes who the project would serve and why a language might be a
good way to meet their needs.

### What's the need?

_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help
them?_

This project would allow teachers and students to assign/submit assignments. Schools currently depend on expensive education software to perform these tasks and having a DSL with this functionality would allow them to perform the same tasks for cheaper with additional customizable features that could be later implemented.

### Why a language?

_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL is appropriate for these users because it would be for students who are slightly older (such that they can operate a computer enough to run a program) and what they would have to run would be fairly easy steps which would be straightforward to use. This addresses the need which technology software (such as gradescope) currently fulfills but it would also promote the use of technical skills to reduce  the need for largely general software which may not address the needs of the specific instructor/class.

### Why you?

_What excites you about this idea? How did you come up with it?_

I am excited about this idea because it is something which can be applicable to a very large poulation, though it has a very specific domain. I came up with it when trying to submit an assignment on Sakai and I reflected on how many complaints I have heard about sakai from instructors and students using it in different ways. I think that this DSL would therefore require deep decisions relating its design as it would be used by many instructors with varying technical skills.

### Domain

_Describe the project's domain in five words._

Education Assignment Management for Schools

### Interface (syntax)

_How might the user interact with the language? What does programming look
like? Why is this the right way to interact with the problem domain?_

The user interaction with the language would depend on the user, which could either be a student or teacher. Though we could imagine scenarios where others may need to review the same information, such as parents, school administrators, or substitute teachers. 

For an instructor, they would reference a file they have stored on their computer and make an assignment object with that such as:

homework1 = Assignment('Desktop/homework1');

Then they could set things like students, release dates, due dates, etc. for that assignment by calling methods such as:

homework1.assignToClass(CS111).release('02-01-2023').due('02-07-2023', '23:59');

For a student they could also use this to submit their assignments by defining it in a similar manner then calling methods as well:

assignment1.submitToClassAndAssignment(CS111, 'Desktop/homework2-07').renameFile('Valdovinos,Christian-Homework2Submission');

I think this is the right way to interact with the problem domain because it would allow users to assign clear dates and other fields which are especially important for assignments which should have clear deadlines and grades associated with them.

### Operation (semantics)

_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program runs, it should act just like a standard Object-oriented language where it performs operations on the values associated with the object, which will likely be mostly on Assignment objects. The program should give clear responses to users on the statuses of assignments, when they are due, if it has been submitted, etc. There would likely be very few errors, like perhaps "Invalid file type" or "Failed to submit".

### Expressiveness

_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to assign, submit, and grade assignments in this language as those are key pieces of functionality which if broken would lead to significant complaints. It should be impossible to get stuck submitting something where you cannot cancel a submission if you begin uploading a very large file that was the incorrect submission.

### Related work

_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

It does not seem like there are any other DSLs in this domain. I looked for DSLs which share this domain however I only found resources on how to teach DSLs or assignments related to DSLs.

## The Project

This section examines whether the idea makes for a good CS 111 project.

### Suitability

_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

If someone were to work on this project, I think that the time could be spent 50% on the language aspects and 50% on the "systems" aspects. Each of these could likely be configured to take longer. However it is reasonable to expect that each of these would take the same amount of time because they both have many considerations to be made.

### Scope

_How big an idea is this? How ambitious is this project?_

I think this is a fairly ambitious project because there are many technical details which may be difficult to implement for the methods. However, it is not a very broad idea and it is limited to the domain of just assignments.

### Benefits and drawbacks

_Why might this be a good idea for a project? Why might this not be a good idea
project?_

I think this is a good idea for a project because it has a limited scope. However, I think it might not be a good idea because many of the technical aspects seem like there could be difficulties implementing and there may be a lot of work required related to design decisions in order to make it broadly applicable for different types of classroom environments. Also, it may lead to worse results than current educational software if the design decisions are not clear.
