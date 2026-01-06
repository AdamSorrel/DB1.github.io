# Wokwi exercise 3: Button Debounce

In this exercise, you should continue in your previous Wokwi workplace. 

## Goal of the exercise

The goal of this short exercise is to implement a simple debounce for your button.


### Blocking code

Start with the blocking code. It is a lot simpler as you can see. Let's see if you can make it work.

```python
while True:
    # Check value of a button.
        # Sleep for some time.
        # Inform user using print
```

### Non-blocking code

Once you have tried the non-blocking code and got it to work, let's up the difficulty a bit. Bellow is a pseudo code for a non-blocking code. It is not that much more complex and it will be very useful for your program. 

```python
from utime import ticks_ms, ticks_diff

# First tiem save time since the last button press using utime's ticks_ms()
while True:
    #Check how much time elapsed since your last button pressed using utime's ticks_diff() function, which has two arguments, t2 and t1
        # If enough time elapsed, check if button is pressed
            # If button is pressed, execute whatever code you'd like
            # Inform user that the button was pressed using the print() function
            # Don't forget to update the time since the last button press here too
```

> [!WARNING]
>  Observe the outcome in the command line carefully. Hopefully, it will work better this time. If you still get multiple clicks, try varying the amount of "idle" time in your code. That is your sleep time or the `ticks_diff()` value. 

Once you have succeeded with a blocking code, try and adjust it to make it non-blocking using the example above. Ask your group peers or a TA if this is not clear. 

> [!IMPORTANT]  
> ## Wokwi final assignment
> Implement a debounced button in your final Workwi assignment. You can also adjust your blinking LED to be non-blocking using the same principle. For now, make your button print a message on the screen. We will learn how to exit your program in one of the upcoming exercises. 