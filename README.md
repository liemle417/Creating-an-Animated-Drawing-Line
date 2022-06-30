# Creating an Animated Drawing Line

Keys to remember in creating an Animated Line Drawing

	Step 1: look for a path and set the "fill" attribute to transparent
	Step 2: in the CSS file, set the stroke and stroke-width
	Step 3: Set stroke-dasharray equal to path’s total length
	Step 4: Set stroke-dashoffset the same as stroke-dasharray
	Step 5: Animate stroke-dasharray to 0
	Step 6: Animate the fill-in when the drawing line is complete 
		@keyframes fill-it{
  	   	   100%{
    			fill: #6fbc6d;
  	   	   }
		}
 

***How do I find the path's total length?
2 ways to find out:

1) I can either set stroke-dasharray with a bunch of number until I can see a full logo. That is not the best way because it is like guessing a number

2) The best way to find out the path's total length is using JavaScript
	var path = document.querySelector('.logo');
	var length = path.getTotalLength();




 
