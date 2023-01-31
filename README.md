# Title - Is your website visible??
Your website is the face of your product. It is literally the first thing anyone will go through if they want to know about you, your company, your services or anything that you represent. It automatically creates a positive impact on anyone who can get in a few clicks.

But have you ever wondered if your website is accessible to everyone? What about the people with disabilities? 

If they can understand, navigate, and interact with your website without any hassle, that makes your product accessible to everyone who is using the web. 

In this talk, I will discuss about what accessibility is, why it is important, who the end users are that get benefitted from it, and finally how to implement it.

## Short Summary

1. Accessibility - What it is, Why it's required?
2. Explanation about WCAG, WAI-ARIA, ADA Compliance.
3. Navigation of a sample website via keyboard
4. Code demonstration of Accessible website using React forms - Semantic tags, labels, Focus management while navigating through keyboard. 
5. Best pratices for Accessibility
6. Testing Tools - Demo on how to use them.
7. Estimated time of talk - 20-30 mins

I am using **React JS** as the primary language for code demo.


## Detailed Explanation

My presentation is divided into 4 parts:

**Part 1**: Introduction - basics of accessibility

**Part 2**: Implementing accessibility on Forms in React - Working code demo.

**Part 3**: Best practices

**Part 4**: Testing accessibility


## Part 1. Introduction
	a. What is accessibility? 
	b. Why is it required?
	c. Who are the end users benefitted from this?
	d. Different types of disabilities - Physical, Visual, Speech, Cognitive 
	e. Simple Demo - How a visually impaired person navigates a website using a keyboard.

## Part 2. Implementing accessibility on Forms in React

**Note for the Organizers**: If a live demo is possible in the conference, I will show the below concepts via coding.
If not, I can take screenshots of the code, record respective output and include everything in the presentation.

I will create 2 forms, FormA and FormB, to demonstrate a thorough example on how accessibility works.
	
**Structure of Forms:**

Both forms will be the same - 4 fields and a Submit button.

a. **Text** - Full name, Email
b. **Drop-down** - Preferred Javascript library/framework (Options = React/ Angular/ Vue.js/ Others)
c. **Radio buttons** - Your Country (Israel, India, UK)

**Difference** - 

1. Form A is a fully-accessible form with all necessary attributes like 
	-	aria-label, 
	-	semantic tags
	- 	focus management
Thus representing how it is perceived by a visually-impaired person. 

2. Form B is without the above mentioned features.

**Form beahviour:** On clicking submit, a pop up will appear asking "Are you sure to submit? ", followed by 2 buttons - Yes / No.
		a. Clicking on Yes will submit the form and display the details.
		b. Clicking on No will return the focus of the screen to the original form with your filled values. 


**Concept 1: Perspective of a visually impaired person**
	
1. I will first demo Form B to show what it lags when we have not complied with accessibility rules.
	-	Navigate the form using keyboard and mouse to show their difference.
	-	Screen reader will be turned on, showing its behavior on different types of fields
	
2. We will be able to hear the respective field names like name, email, etc, thus demonstrating importance of semantic tags.
	
3. After this, I will navigate through the Form A to show the correct implementation.
	
**Concept 2: Managing and trapping focus**

	1. During the demo of above Concept 1, I will also show how focus moves when navigating through the keyboard.
	2. This will be done by creating a fixed 1px border around the focused content.
	3. After clicking submit, when pop-up appears, I will show how focus moves when the pop-up is opened and closed. 
	4. I will also demo how to trap the focus inside the pop-up.
	5. Discussion on “tabindex” attribute
		a. Values that can be assigned to it
		b. Explanation of why tabindex = 0 is important.
		c. Effects of using tabindex = -1 , tabindex = 1
		
## Part 3. Best practices (3-4 mins)
	1. Importance of semantic tags.
	2. How to choose the right contrast and colors.
	3. Brief about a11y and how to use it correctly.

## Part 4: Testing accessibility (3-4 mins)
	1. Axe tool - how it works, meaning of the score given by it, how to improve your website from the given score.
	2. Writing unit test cases for accessibility.
	3. Popular screen readers and how to use them.
