[Exercise Instructions Video](https://youtu.be/FdIrVm9lOmY)

## Project Instructions
new Date() gets the current date. Running getTime() on the current date converts it to milliseconds, which you want to work in.
    
You want to get the final countdown time/date. 

You want to use JavaScript's setInterval method to run a function every second (or 1000 ms)

In that function you want to get the current time/date, compare it with the final coundown time/date, and put that in a variable. 

Then you need to do some millisecond conversions with your remaining time to put it back into "human" format. There is no magic here....just math. And it's this:
    var days = Math.floor(remainingTime / (1000 * 60 * 60 * 24));
    var hours = Math.floor((remainingTime % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    var minutes = Math.floor((remainingTime % (1000 * 60 * 60)) / (1000 * 60));
    var seconds = Math.floor((remainingTime % (1000 * 60)) / 1000);

Then you want to use JavaScript to display that on your page. 

Finally, you want to be sure to change the message when the timer runs out. 

<h3>My Final Code</h3>
Please don't check the solution in the solutions-dont-peek folder until you've wrestled with the outcome and solved it. You will learn so much through this process. But after you have a working solution, feel free to compare.