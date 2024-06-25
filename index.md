# Bluestamp Ball Tracking Robot
This is my journey in the Bluestamp engineering program to create a robot that can follow a red ball. Potential additions in the future may include voice command and AI recognition!

<!---You should comment out all portions of your portfolio that you have not completed yet, as well as any instructions:-->



| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Aaron L | Diamond Bar High School | Electrical Engineering | Incoming Senior

<!--- **Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.** -->

![Headstone Image](logo.svg)

<!---
# Final Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE
-->


# First Milestone - Wiring and Testing

<iframe width="560" height="315" src="https://www.youtube.com/watch?v=AWm2tbdo_Qw&list=PLe-u_DjFx7eticgHvdNBMS-CTTohSGwUM&index=10" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

This project involves the raspberry pi, which I last used when I was 6, back in 2013. It also includes using motors and ultrasonic sensors, so there is great value to be had undertaking this project. However, this project isn't simple. 
- This project requires some knowledge on how to use a raspberry pi and its OS, along with sufficient knowledge on how circuits work. Specifically, a raspberry pi, ultrasonic sensor, motors, and electrical circuiting was used in this project.
- So far, the wiring is fairly simple, wiring the power source to the breadboard to the rest of the components, and the code is simple, with the GPIO system on a raspberry pi being well documented. Picamera2 was new to me, but was trivial to implement. Future additions may introduce more of a challenge, such as tensorflow lite or pose recognition, which utilize the components I already have, but are more complicated to implement.
- With that being said, mistakes were certainly made. Over these 5 days, I spent 1 of them rewiring because of an error in orientation of the raspberry pi. I definitely learned to be even more meticulous than I already was and am confident I can handle these situations in the future.
- With two more weeks to go, immediate goals include finishing the code to have the robot autonomously track a target. Beyond that, implementing more complicated systems with code onto the raspberry pi is very attractive, while physical modifications are likely unnecessary beyond improving the basic functioning of the robot. 

# Second Milestone - Code and Tuning

<iframe width="560" height="315" src="https://www.youtube.com/watch?v=1GEd_ZLxvUk&list=PLe-u_DjFx7eticgHvdNBMS-CTTohSGwUM&index=28" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

This project uses relatively simple code and structures. The pain comes from changing threshhold values. 
- Before starting anything else, I had to neatly rewire everything so if any errors come up, I can blame something other than the wires. 
- A pseudo code phase is helpful, but I broke down the process into two parts: Look for the ball, move towards/away from the ball. I completed the first part in this milestone. 
- After setting up the base code, I ran the code and to no one's surprise, nothing worked. Either the camera values were too vague and there was too much interference, the motor wiring was swapped, or the ultrasonic sensors were too inconsistent, I had to fix the errors as they came up, not in preparation for them. 
- Because of this, this step took a whole week. However, I'm proud to say that the robot can consistently track the ball. The next milestone will include the second step previously mentioned, keeping the robot a certain distance from the ball. 

<!---
# Final Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE
-->

<!---
# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 
-->

<!---
# Code
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 
-->
<!---
```c++
void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  Serial.println("Hello World!");
}

void loop() {
  // put your main code here, to run repeatedly:

}
```
-->
<!---
# Bill of Materials
Here's where you'll list the parts in your project. To add more rows, just copy and paste the example rows below.
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
-->

<!---
# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)
-->
