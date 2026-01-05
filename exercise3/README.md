# Wokwi exercise 3: Button Debounce

In this exercise, you should continue in your previous Wokwi workplace. 

## Goal of the exercise

The goal of this short exercise is to implement a simple debounce for your button.

You can with the easier example of a blocking code.

| Blocking code | Non-blocking code | 
| ------ | ------------- | 
| <img src="./ex3imgs/blockingCode.png" alt="Blocking code"> | <img src="./ex3imgs/nonBlockingCode.png" alt="Blocking code">

> [!WARNING]
>  Observe the outcome in the command line carefully. Hopefully, it will work better this time. If you still get multiple clicks, try varying the amount of "idle" time in your code. That is your sleep time or the `ticks_diff()` value. 

Once you have succeeded with a blocking code, try and adjust it to make it non-blocking using the example above. Ask your group peers or a TA if this is not clear. 

> [!IMPORTANT]  
> ## Wokwi final exercise
> Implement a debounced button in your final Workwi assignment. You can also adjust your blinking LED to be non-blocking using the same principle. For now, make your button print a message on the screen. We will learn how to exit your program in the next exercise. 