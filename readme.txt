******1 thing Very Important*******

Line number 52 of UserMain.java- 	p = Pattern.compile("^\\d{10}$"); // For US use this "\\([4-6]{1}[0-9]{2}\\) [0-9]{3}\\-[0-9]{4}$"
You can implement this pattern as per your local US mobile numbers - I have implemented for INDIA format but in comments you can find my suggesstion for US 
Please test this phone Number after you modify for US , remove india pattern

*******************


Main Class to run : UserMain.java

Implemented Design Patterns :
Builder --> Files to refer UserMain, User.java, UserBuilder.java, DonorBuilder and RecipientBuilder.java

Singleton --> Refer User.java

Composite --> Refer UserMain.java, Applicants.java (Component), TotalApplicants.java(Composite), leaf's (DonorBuilder and RecipientBuilder.java)

Bridge --> Refer UserMain.java, WHO (abstraction class), DonorOrganBank & Recipient OrganBank (Refined abstraction), OrganBank (Interface as IMPLEMENTOR)
           , DonorBuilder and RecipientBuilder.java (as Concrete Implementations).
		   
-------------------------------------------------------------------		   
Junit 4.13 is used for Test cases
------------------------------------------------------------------------
Compiling and running in eclipse

1. Extract and import this module into eclipse
2. Run UserMain.java as a java application

---------------------------------------------------------------------------------
Jar generation steps from eclipse-
Right click on the project , click on Export option, expand java folder in pop up, select jar, give the destination for the jar to save in your local
click Finish

-----------------------------------------------------------------------
Compiling and running the application using command prompt

Go to run --> type cmd -->

Go to the path of your jar file download from this project

Execute the below command from command Line and verify the application

java -cp Organ-Donor-Receipient.jar com.organ.user.main.UserMain

------------------test cases --------------

Builder and Singleton test cases are written and tested using junit 4.13 under package com.organ.unit.tests

Import the project into eclipse and Just right on the file and click on run as Junit from eclipse.



-------------Git---------

The entire project is pushed to git hub  in this path - clone it
This package cloned will also have the jar file preconstructed.

----------------------
