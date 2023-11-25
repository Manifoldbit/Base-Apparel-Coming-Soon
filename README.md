# Frontend Mentor - Ping coming soon page solution

This is a solution to the [Ping coming soon page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/ping-single-column-coming-soon-page-5cadd051fec04111f7b848da). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page
- Submit their email address using an `input` field
- Receive an error message when the `form` is submitted if:
	- The `input` field is empty. The message for this error should say *"Whoops! It looks like you forgot to add your email"*
	- The email address is not formatted correctly (i.e. a correct email address should have this structure: `name@host.tld`). The message for this error should say *"Please provide a valid email address"*

### Screenshot

![](./screenshot.jpg)


### Links

- Solution URL: [https://github.com/Manifoldbit/Base-Apparel-Coming-Soon.git]
- Live Site URL: []

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- Javascript

### What I learned

In this project i was able to learn how to use form validation with javascript using regular expression

some examples of code snippet below:

```css
.image{
  visibility:hidden; 
}
It helps me hide my mobile image from reflecting in desktop size
```
```js
function validateEmail(){

    if (emailField.value == ""){
        emailError.innerHTML = "Whoops! It looks like you forgot to add your email";
        emailField.style.border = "1px solid red";
        emailError.style.right = "53%";
        return false;
    }

    else if(!emailField.value.match(/^[A-Za-z\._\-0-9]*[@][A-Za-z]*[\.][a-z]{2,4}$/)){
        emailError.innerHTML = "Please provide a valid email address";
        emailField.style.border = "1px solid red";
        emailError.style.right = "60%";
        return false;
    }


    else{
        emailError.innerHTML = "";
        emailField.style.border= "1px solid green";
        alert("You will be notified");
       
        return true;
    }
    This code snippet helps to validate an email, IF the email input is wrong then, u will see a message that says "Please provide a valid email address";
    IF the email input is empty, then you get a message that says "Whoops! It looks like you forgot to add your email";
    but IF the email input is correct , then you will get a an alert box messsage that says "You will be notified soon"
```

### Continued development

Basically I want to continue learning and developing my Javascript skill, this is the first project i will make use of javascript, so i want to keep learning and be so build more advanced project with HTML, CSS and JAVASCRIPT

### Useful resources

- [Example resource 1](https://www.youtube.com/watch?v=ndNPg8-5jgI) - This is an amazing video tutorial that helped me to use javascript for form/email validation.

## Author

- Website - [Manifoldbit](https://Manifoldbit.com)
- Frontend Mentor - [@Manifoldbit](https://www.frontendmentor.io/profile/Manifoldbit)
- Twitter - [@bit_codes](https://twitter.com/IloriBabajide)

