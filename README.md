Github link: https://github.com/nkn5310/Voter-Registration/tree/main 

 

Goal: The goal of this code is to create a simple voter registration and management system. In this code, users can simulate the process of registering to vote for the first time. Existing users can also modify their voting information. Although this code is quite simple in functionality, this can be used in an actual voter database and operate in a real-world situation.  

Significance: This project highlights how coding projects can be important and useful in real life. The diversity of python projects is infinite which is why I enjoy doing personal projdects lile these. Even though this code is meant for elections, it could easily be modified to handle different situations such as employee databases for companies or authorization and authentication for security. 

 

The beginning of the code will first ask the user if they are a first time voter or not. 

If the user answer yes (y), they will be asked to provide personal details such as full name, date of birth, county, and political party. 

After the user enters their personal information, they will have successfully registered to vote. The voter’s details will be printed for the user to see. 

 

If the user answers no (n), it is assumed that the voter is already registered to vote. If a user is a returning voter and is already registered, their information should already exist in the database. The user is asked to login using their personal information. After entering the existing voter’s information, the voter has 2 options to choose from. They can either view their existing details or they can change their current voter information. 

If a user chooses to view their information, all of their information will be displayed for the user to see. If a user chooses to update their information, a user can update any attribute of their voter details. 

 

Structure: 

The bulk of the code is managed inside of the Vote Class. This is where a voter object is created with personal information attributes such as full name, date of birth, county, and political party. When the user is asked to enter their date of birth, a method called is_18_or_older checks to see if the voter is at least 18 years old. If the user is not 18 year old or older, the code stops. If the user is at least 18 years old, they will proceed to entering their information.  

Their is a database of existing voters named exisitng_voters. It is a list filled with Vote objects that are meant to simulate existing voters in the system. When an existing voter goes to login using the login method, their personal information will be used to verify that a user already exists. If their information has not been found, the code will return ”Voter not found” 

If their information has been successfully found, the user can then view their details or update them. The display_details method makes this possible. The update_details method lets users change or keep their voting information.After making changes to the voter information, the users updated information will display. 

 

 

 

 

 

 

 

 

 

 

 

 

 

Extra details + issues faced 

 

Some issues I faced when doing this project included making the login method. The reason for adding a login method was to test whether or not a user was already an existing voter or not. When I was creating the Vote class, I wanted users to be able to modify their voter information even after creating the object. In order for a user to be able to modify their details, the user would have to exist already. This is the reason why I added the list of users called existing_voters. I created two voters named John Doe and Jane Doe. 

 While logging into the voter registration, you must use the exact information as John Doe. The code will make sure their details match exaclty. If the information matches, John Doe can proceed to making changes.  
