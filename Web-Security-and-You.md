---
title: Web Security and You
layout: post
author: rmerino
permalink: /web-security-and-you/
source-id: 1uLQ2CK32mhnKpcWp9QYkmOj8SR2zw0ahsNoFf7OBX4I
published: true
---
Web Security and You

Eli White | @EliW

## The Open Web Application Security Project

* [http://owasp.com](http://owasp.com)

    * The best online resource for learning about various attach vectors and solutions to them

## Password Hashing

* Don't store plain text

* always 1-way hash

* do not just use md5

* don't even use SHA-1 or SHA-512

    * The longer your hashing takes to run, the longer it takes for someone to crack it

* Generally a hash should take time

## Password Hashing -- PHP 5.5

[http://php.net/password](http://php.net/password) `password_hash` PASSWORD_DEFAULT constant uses the latest password hashing algorythm. 3rd argument is an array of options, `cost` the higher the cost the longer the hash takes.

## SQL Injection

A user having the ability to send data that is directly interpreted by your SQL engine.

Uings PDO solves attacks by using `$query->prepare( ... 

### Other Injections

* Command injection

    * the user being able to inject code into a command line.

* Unchecked File Uploads

    * The user being allowed to upload an executable file.

* Code Injection

    * User being able to directly inject code (don't use eval!)

## Session Hijacking

One user 'becoming` another another user by impersonation

* Session Fixation

    * The Attack: example.com/?PHPSESSION=abc123

    * The Solution: 

        * Use cookies

    * Any time you change and access level regenerate the session ID. This destroys the old one

### Session Anti-Hijack Measures

* Use anti-hijack measures to ensure user is legit

    * Not a few lines of code

        * Store whatever unique you can about the user/browser combination to verify the user

    * When starting a session sent the user a session id along with a token that they have to send back later to continue the session.

## XSS (Cross Site Scripting)

A user sending data that is executed as script

* Don't trust the user!!!

* Don't forget about rewritten URL strings!

### XSS - Reflected XSS

Directly echoing back content the user entered.

* The solution

    * HTML -> htmlentities

    * JS -> str_replace, add_slassges

### XSS - Stored

You store the data, the later display it. The fix is the same as reflected XSS.

### XSS - DOM XSS

chrisisbeef/jquery-encoder -> scapes HTML and CSS to prevent Javascript attaches

### XSS - CSRF

User submits a request on behalf of someone else

Solution generate token with session and submit as hidden field in form, on submition you check for the token

## Server Security

No Excuses. Keep all your software up to date.

## DDOS & Similar attacks

rely on firewall features of your machine & hosting. Hire a good ops team.

[https://www.phparch.com](https://www.phparch.com)

http://musketeers.me

