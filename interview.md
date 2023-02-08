# Interview project

## The user and a language

This section describes who the project would serve and why a language might be a
good way to meet their needs.

### What's the need?

_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help
them?_

This project meets the needs of researchers who want to set up their study designs. Currently researchers can access online websites which allow them to input values for the number of subjects they have, the number of groups they will have, and the number of participants they want to assign to each group. This then outputs which person's number (like an ID) is assigned to which groups. However, this is inconvenient because they have to manually return to their list of participants and attach the groups that the website output to each participant. It would improve their experience to use this tool because we could return tuples of the participant name/contact info, and the group they were assigned to.

### Why a language?

_Why is a DSL appropriate for your user(s)? How does it address the need?_

This DSL is appropriate for researchers because it allows them to have a more effective process for conducting high quality research. This is a process they have to perform anyways for research and by decreasing the barriers for doing repetitive processes like this group assignment in experiments, researchers can dedicate more time to the aspects of the experiment which require more attentive effort, like the methodology and analysis.

### Why you?

_What excites you about this idea? How did you come up with it?_

This idea excites me because it is a simple task which may be very repetitive in the field of research. I came up with it by interviewing a psychology student who discussed their experience with experiments and what some of the procedures for that are.

### Domain

_Describe the project's domain in five words._

Experiment Random Sampling and Assignment

### Interface (syntax)

_How might the user interact with the language? What does programming look
like? Why is this the right way to interact with the problem domain?_

The user might interact with this language by writing short lines of code which are each separate and each define a different part of the experiment. I think it would look like the following:

participants = ['Mary', 'John', ... ];

assignment random;
groups ['Control', 'Experimental Group 1', 'Experimental Group 2'];

Then users would be output a sequence of tuples or a table in a file like an excel sheet or even a pdf of the groups and/or the list of participants with the groups.

The example above would evenly distribute participants into the three groups but we could also do other forms of sampling assignment, such as stratified where every kth person is assigned to a group or clusted where the first, second, and third thirds of the participants are assigned to each group.

### Operation (semantics)

_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program runs, it would look for a list of participants, a command for assignment (and possibly for sampling), and finally the groups which each person should be assigned to. There could be errors like where two people have the same name and thus it could be unclear which is assigned to each group but we could communicate this by saying things like "Participants invalid. Ambiguous naming: there exist multiple instances of 'Mary'".

### Expressiveness

_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to input categories of approaches for sampling/assignment and also quantities, in case you want to assign a certain number of people to each group, or only use X of the participants. It should be impossible to circumvent the randomness of the output group because that could lead to faulty experiment designs due to a DSL flaw.

### Related work

_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There do not seem to be any other DSLs in this domain, there are DSLs for vizualizing data after an experiment has been conducted but I found none related to experiment design. I assume this is because researchers are fairly satisfied with their current approaches and it is a much easier process than much of the methodoogy or data analysis that they have to conduct.

## The Project

This section examines whether the idea makes for a good CS 111 project.

### Suitability

_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

If someone were to work on this project, since the language aspect is so simplified, I would assume it'd be aprroximately (1/3) or 33% of the time spent on the project while the remaining 67% percent would be for the "systems" aspects of the DSL.

### Scope

_How big an idea is this? How ambitious is this project?_

This is not a very big idea as the project is very limited in scope so I would consider this a reasonable project for the course.

### Benefits and drawbacks

_Why might this be a good idea for a project? Why might this not be a good idea
project?_

This might be a good idea for a project because it allows for a lot of design considerations since the scope is limited to the task of experimental sampling and assignment. However, it might not be a good idea because it may involve a large amount of work on trying to make sure that the input commands are error-free to avoid outputs not representing the limited code written by the user.