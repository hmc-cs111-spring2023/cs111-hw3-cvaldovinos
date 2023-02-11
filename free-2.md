# Free project 2

## The user and a language

This section describes who the project would serve and why a language might be a
good way to meet their needs.

### What's the need?

_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help
them?_

This project would help economists and economics students perform calculations using some of the formulas in Excel or Google Sheets. Currently, if an economist wants to perform one calculation given some variables, they have to do it by hand, find a calculator on an odd website (many of which use different formulas), open up a new Excel file or a Google sheet just for that one line calculation.

### Why a language?

_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL is appropriate for users because it would address the needs of trying to apply the same formula while changing a few variables and the users would be used to inputting the formulas in similar manners so they should have sufficient technical background to put variables into a format.

### Why you?

_What excites you about this idea? How did you come up with it?_

I came up with this idea because I was in my Behavioral Finance class when I was trying to recall a formula, then I remembered how bothersome it has been in the past doing ECON homework assignments and having to create google sheets and select cells spead out just to show my work on how I used variables in a function. This project idea excites me because it is something I know that I have wanted and it will help others in the future, making repetitive processes simpler and acting similar to tools like wolfram alpha which help mathematicians, improving the quality of the work in that field.

### Domain

_Describe the project's domain in five words._

Economic and Finance Formula Calculations 

### Interface (syntax)

_How might the user interact with the language? What does programming look
like? Why is this the right way to interact with the problem domain?_

The user could interact with the language similar to calling formulas in general purpose languages. However, it should remove many of the technical concepts that economists may not have the understanding of when writing in this language.

### Operation (semantics)

_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program runs, it should output things just in the console. I would expect it to be much like a standard calculator and thus it should have very basic error handling that people with understanding of algebra/calculus should be able to understand such as: "division by zero error", "Invalid value for X", and "Not enough variables. This function expects the following variables: X, Y, and Z".

### Expressiveness

_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

This DSL should allow you to easily construct lists such as of years, quantities, and perform standard operations and some of the basic ECON formulas in google sheets such as: SUM(), PV(), VARIANCE(). This also means it should be possible to do basic arithmetic operations +,-,*,/. I think the expressiveness of the DSL should be limited mostly to these things so it should likely not be possible to do other things so that people will not be confused or led to believe there is additional behavior they can engage in.

### Related work

_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

It does not seem as if there are any other DSLs in this domain. There are other math-related programming languages such as MATLAB and R. However, these languages both have many pieces of functionality that are common among languages we would consider general purpose programming languages. Additionally these languages' domains are more generally mathematics so they are more broad than the scope of the issues I seek to address with this project.

## The Project

This section examines whether the idea makes for a good CS 111 project.

### Suitability

_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

Because many of the formulas economists use are standard across tools such as Excel and Google Sheets, there would not be many design decisions to make as we would want to maintain most of the standard practices and ensure that the "systems" aspects are fully functional. Thus I would say 25% of time on the language and 75% of the time on the "systems".
### Scope

_How big an idea is this? How ambitious is this project?_

I think that this project is not very ambitious. Particularly because it would be best to slowly introduce features, this project could include as many functions as can be implemented but the primary focus would be on handling errors, displaying information, and making the DSL easily usable.

### Benefits and drawbacks

_Why might this be a good idea for a project? Why might this not be a good idea
project?_

I think this is a good idea for a project because it is domain specific to a domain outside of CS though it uses the convention of calling functions with variables which we are very used to doing with general purpose programming languages. Additionally, it requires less design decisions since it is related to pre-existing tools. However, it might not be a good idea because depending on how difficult it is to implement the language to be callable, it could end up as a more complex tool to use in comparison to the standard implemented in Excel and Google Sheets.