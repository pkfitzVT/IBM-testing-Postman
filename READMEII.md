Curl Testing for PC Power Shell
curl.exe localhost:5000/user

//Identified record from email
curl.exe localhost:5000/user/johnsmith@gamil.com

//Uses post to insert a user to the variable
curl.exe --request POST 'localhost:5000/user?firstName=Jon&lastName=Lovato&email=jonlovato@theworld.com&DOB=10/10/1995'

//Verify user insert
curl.exe localhost:5000/user/jonlovato@theworld.com

//Changes the dob value to the record matching the email
curl.exe --request PUT 'localhost:5000/user/johnsmith@gamil.com?DOB=1/1/1971'

//verifty user
curl.exe localhost:5000/user/johnsmith@gamil.com

//Delete method
curl.exe --request DELETE 'localhost:5000/user/johnsmith@gamil.com'

Using Postman
base url
http://localhost:5000/

set get in menu
http://localhost:5000/user

//returns the contents of the variable
http://localhost:5000/user/johnsmith@gamil.com

//tests post
http://localhost:5000/user?firstName=Jon&lastName=Lovato&email=jonlovato@theworld.com&DOB=10/10/1995'

//tests put
localhost:5000/user/johnsmith@gamil.com?DOB=1/1/1971'


