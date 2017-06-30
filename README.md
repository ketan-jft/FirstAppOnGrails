# FirstAppOnGrails
How to create an application in grails Example with Notes by Ketan Pandey. Special thanks to my Seniors
﻿Create Apps on Grails
Step 1 : Run Following Command :
	grails create-app app_name
	cd app_name
	grails run-app
Step 2 : Create Domain Class under a package
	grails create-domain-class com.firstApp.User
	package com.firstApp
	class User {
	    String username;
	    String password;
	    String email;
	    static constraints = {
	        email email: true;
	    }
	}
Step 3 : Generate Controller
grails generate-controller com.firstApp.User
static scaffold = true; // Write in UserController class
Step 4 : Generate View
grails generate-view com.firstApp.User
Step 5 : Run App
grails run-app
