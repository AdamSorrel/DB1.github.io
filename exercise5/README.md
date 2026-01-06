# Wokwi exercise 5: Breaking a loop

You will be using infinite loop in your programming project to keep acquiring data indefinitely, however it is important to be able to interrupt this loop for example to safely disconnect from your device. This is important, because trying to disconnect while the device is writing into your file would corrupt your data and render them unreadable. 

## Breaking loop syntax

To break a loop in python, we use a statement `break`. This is not a variable, nor is it a function, which means that it is **not written with parantheses `()`**. A simple synthax using the `break` statement could look as follows:

```python
n = 0
while True:
    n = n + 1
    if n > 3:
        print("n is too high now!")
        break
```
This loop will be incrementing a variable `n` by one in each iteration and when it gets to 3, it will exit the loop.

> [!NOTE]
> This is not the most sensible way to code the behaviour above. If you have any experience with python's `while` loop, you would know that it would make a lot more sense to add the condition e.g. `n < 5` into the while statement, this only meant to illustrate the use of the `break` statement on a simple case.

> [!CAUTION]
> Make sure your indentation is correct. Python is very sensitive to indentation as it describes what belong where. Note the following loop:
> ```python
>n = 0
>while True:
>   n = n + 1
>   if n > 3:
>       print("n is too high now!")
>   break
> ```
> This loop will only run once. At the end of its first run it will encounter a `beak` statement and exit. At that point `n` will have been equal to 1. 

## Breaking a loop with button

Let's create a script that contains an infinite loop that blinks an LED at your desired frequency. Earlier today, we have worked with buttons and how to debounce them properly. Use some of your previous code to arrange a program where a user pressing a button will trigger a `break` statement. Make sure to implement your button debounced. 

You can start from this Wokwi example: [https://wokwi.com/projects/452401289665340417](https://wokwi.com/projects/452401289665340417)

> [!TIP]
> You might notice that your button does not react particularly well. Depending on what LED blinking frequency you have chosen and how you have implemented it, it might take a while for the button state to get evaluated. 
> 
> We have previously talked about a non-blocking implementation of a button debounce. Can you implement a non-blocking LED blinking using the same method?

## What happens after a loop is exitted

In your previous example, your program has probably exitted right after you have broken out from your loop. However, it is important to note that breaking or exitting a loop is **not the same** as exitting your whole program. If there is any code after the loop you have exitted, it will get executed after you broke from the loop above it.

We will play around with this concept now. Take the program you have written above and add another infinite `while` loop after the first one you have just written. You can also add additional LED and start blinking that one, or perhaps change the frequency of blinking on the original one. Either way, make sure that both of your loops produce a notable effect. Upon pressing the button, the first loop should exit and the second loop will then activate afterwards. 

> [!NOTE]
> You can think about your first loop as a waiting loop. When you are setting  your device, perhaps you want to make sure everythign is in place first. You might even want to check that your detection orange LED is working properly, but you probably do not want to acquire any data yet while settings things up. This is where a "waiting loop" comes in handy. 

> [!TIP]
> Done before the allocated exercise time? You should now be able to connect to your HUZZAH32. Why not trying to test some of your code in your actual device if you have the time? Start with a simple LED blinking perhaps. You can even use the internal LED, which on HUZZAH32 is connected to the pin 13. That way you don't have to do any wiring for now. See if you can do that and ask TAs for help if you run into troubles. 

---
> [!IMPORTANT]  
> ## Wokwi final assignment
> Return to your final Wokwi assignment. At this moment you should have implemented an LED and a button, which is hopefully correctly debounced and pressing it prints a message through the serial monitor. Edit your code such that your loop will exit upon pressing the button as well. Moreover, add another loop, which will also be exitted with a second press of the same button. To notify the user that you have entered a new loop, you can perhaps change the frequency of the indicator LED blinking or add additional LED. 
>
> You are highly encouraged to be creative, explore all possibilities and play around during your exercise. Unfortunately, your Wokwi assignment needs to adhere to a certain structure in order to be feasible to evaluate. You are thus required to follow the required structure of the assignment. This limits the number of LEDs to 2. Indicator LED and an orange detection LED which will be added later and the number of buttons to 1. 