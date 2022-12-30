My presentation is divided into 4 parts:
Part 1: Introduction - basics about accessibility
Part 2: Implementing accessibility on Forms in React - Working code demo.
Part 3: Best practices
Part 4: Testing accessibility

Detailed explanation is given below.

## Part 1. Introduction (approx 3 minutes)
	a. What is accessibility? 
	b. Why is it required?
	c. Who are the end users benefitted from this?
	d. Different types of accessibility requirements
		- navigation through keyboard, 
		- contrast, 
		- stressful vs soothing color-combination example.

## Part 2. Implementing accessibility on Forms in React (10-15 mins)

Note: If a live demo is possible in the conference, I will show the below concepts via coding.
If not, I will take screenshots of the code, record respective output and include everything in the presentation.

 **Concept 1: Perspective of a visually impaired person**

	1. I will create 2 forms to demonstrate a thorough example on how accessibility works.
	2. Form A is a fully-accessible form with all necessary attributes like aria-label, semantic tags and focus management, thus representing how it is perceived by a blind person. Form B is without the above mentioned features.
	3. Form structure - Both forms will be the same.
	
  It contains 4 fields and a Submit button.
		a. Text - Full name, Email
		b. Radio buttons - Preferred Javascript library/framework (Options = React/ Angular/ Vue.js/ Others)
		c. Drop-down - City (10 random cities from England)
		d. on clicking submit, a pop up will appear asking "Are you sure to submit? ", followed by 2 buttons - Yes / No.
	
	4. I will first navigate through Form B to show what it lags if we have not used accessibility features.
	5. Entire navigation will be done using keyboard only, showing the behavior of the screen reader on different types of fields.
	6. We will be able to hear the respective field names like name, email, etc. This will demonstrate the importance of semantic tags.
	7. After this, I will navigate through the Form A to show the correct implementation.
	
**Concept 2: Managing and trapping focus**
	
		1. During the representation of above Concept 1, I will also show how focus moves when navigating through the keyboard. 
		This will be done by creating a fixed 1px border around the focused content.
		2. After clicking submit, when the pop-up appears, I will show how the focus moves when the pop-up is opened and closed. I will also demo how to trap the focus inside the pop-up.
		3. Discussion on “tabindex” attribute
			a. values that can be assigned to it
			b. explanation of why tabindex = 0 is important and ideally should not be assigned any other value if we want to focus on the content 
			c. Effects of using tabindex = -1 , tabindex = 1
		
## Part 3. Best practices 
	a. Importance of semantics
	b. How to choose the right contrast and colors
	c. Brief about a11y and how to use it correctly.

## Part 4: Testing accessibility
	a. Axe tool - how it works, meaning of the score given by it, how to improve your website from the given score.
	b. writing unit test cases for accessibility.
	C. Popular screen readers and how to use them.
