# IT2163-ApplicationSecurityAssignment
Admin no.: 201922D \
Name: Muhammad Arif Bin Hamed \
Module group no.: 07



## Changelog
#### Update 1.0.0
* Create and upload to Github with ASP.NET Web Application empty project from\
Visual Studio 2019

#### Update 1.0.1
* Created Registration & Login
    * Registration:
        * All inputs are set
    * Login
        * Empty web page for now

#### Update 1.0.2
* Updated README.md

#### Update 1.0.3
* Added sql file to a Database Folder
    * Might consider moving that file somewhere else more secure
* Added more to Registration server-side code
    * DOB and card details
    * Changed Email to be ID

#### Update 1.0.4
* Updated Login
    * Added Login via Email & Password textboxes
    * Not including captcha yet
* Updated Registration
    * Changed from using Width so much to using table with boostrap
    * Major edits to server-side code
* Issues
    * Probably existing error in checkPassword function in Registration

#### Update 1.1.0
* Major changes
    * Changed mdf location
        * From Local SQL
        * To App_Data file in repo
        * Change is inherited from Practical 7
    * Database changes
        * I gave up and replaced almost everything into string, cuz nah, i can't deal with that whole datetime bs anymore
    * Fixes to Registration.aspx
        * With database fix, registration is now functional
    * Added ServerText
        * Used as a generic text feeder for users
* Current issues
    * Registration.aspx
        * Validation for length isn't auto checked by client-side javascript

#### Update 1.1.1
* UI
    * Minor aesthetic update
        * Increased font size for some words for readability
            * Registration
            * ServerText
* Added reCAPTCHA v3 into Registration
    * lads and geens, the captcha is functional.
* ServerText
    * Added meta tag to redirect to login (for now)

#### Update 1.1.1b
* Designer cs update
    * These updates may be common, as the local repo is edited on an NTFS usb drive, and I do move around time to time with this laptop in my bag, but i also don't want to damage the usb drive. so here it is i guess.

#### Update 1.1.1c
* Update csproj to stop showing something that doesn't exist, like a reference to the lyrics of I Miss You by Blink 182.

#### Update 1.1.2
* Login
    * Added in captcha v3 derived from registration
    * Updated TextMode for the password field to Password
    * Updated functional login (with hash and salt). 
        * Basic login successful!
    * Added email verification fields (NOT FUNCTIONAL YET)
* Home
    * Created as home page to change stuff
* Error page
    * Defaults all errors to that page (pls enable in demo)
* Current issues/future fixes
    * Validations
        * Verify email in registration, possibly with SMTP
    * Account lockout after 3 failures
    * Audit log
    * Implement SQLi and XSS prevention
    * Account policies
        * Automatic account recovery after x minutes of lockout
        * Avoid password reuse (max 2 password history)
        * Change password
        * Minimum and maximum password age (cannot change password within x minutes form the last change of password and must change password after x minutes
    * Github checking thingy
    * Add in db modification in Home

#### Update 1.1.2b
* Minor warm-up update
    * Started to work on functionality on these
        * Account lockout
            * Login.aspx.cs:77
        * Photo upload
            * Registration.aspx.cs:189
    * Changed accounts table values (and deleted pre-exisiting data)
        * Added "Lockout"









