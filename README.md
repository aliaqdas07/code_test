# Code Test
This project is a test project created for [Digitaltolk](www.digitaltolk.se).
## Thoughts about controllers

Overall `repository pattern` is a very good approach to make separate layers of data and business logic. While it also make easier for unit testing of application.
<br />
`$request->__authenticatedUser` this I am assuming as private property defined on request.
<br />
`Responses` should be well structured, mean need to return response with proper key values, like `message, success, responseCode`.
<br />
`Unused code` this type of code should be commented or not should there.

## Thoughts about Repository

In the `getUsersJobs` on model `is` function is used to check two instances of same model, but that was using to check for user type, so i am assuming user type as role.
<br />
`Repository` have alot of junk code and conditions which can be optimize alot. But i am refactoring some and putting comments in some places which can be more optimize.
<br />
Overall which i see is that there are queries duplications and in a single function there is alot of logic, which should be moved to small small chunks and other things like `model scope` and static functions we should use.
<br />
And there should be a `helper class functions` to check for the date diff and other calculations.
