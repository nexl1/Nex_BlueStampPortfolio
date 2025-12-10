# International Space Station Tracker
November 20, 1998 marks the date of the first ISS segment launched into orbit. Since then, humanity has sent over 40 assembly flights and spent over 1,000 hours space walking to construct the International Space Station. Today it stands as an epitome of space innovation, technology, and collaboration, harboring 9 astronauts and granting a safe and stable location to perform numerous experiments and research. My project will not only allow users to track the live location of the ISS, but will also creat a predicted path for the space station, giving the world below a glimpse at the endless possiblities in the stars above their heads. 

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Nex L | Portola High School | Astrophysics | Incoming Senior |


![Headstone Image](logo.svg)
  
# Final Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE
For my third milestone, I completed my second modification and added final touches to the International Space Station tracker. I 


# Second Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/6hgNIT6npPA?si=8hoHP8ag0Wfsjzr4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

For my second milestone, I was able to complete my first modification. I added a prediction line using an SGP4 algorithm to calculate the predicted path of the International Space Station (ISS). I also switched to a Raspberry Pi Model 4B with a 7" LCD Display Screen to display the project. Now the project displays a 400x240 sized map that contains the current location in red, trail in yellow, and prediction line in green. I faced many challenges throughout this milestone and that first began with solving for the predicted path. I did some research on how to predict the path of the ISS, and I found some interesting information regarding the topic. 

Two Line Element set (TLE) is 2 lines of numbers that can be translated into important information about an astral object orbiting the Earth, such as the mean motion, inclination, and eccentricity. I initially couldn't understand much of this information because I didn't have much advanced mechanics physics knowledge, but I soon found out how to utilize data from the TLE. The Simplified General Perturbations Model 4 (SGP4) is an algorithm that can perform orbital determination topics. Since I struggled to figure out the higher-level physics and math concepts, I utilized phython and downloaded the SGP4 library online. Through this, I was able to understand the algorithm better and ultimately use it in my code. Now, in my virtual enviornment, I was able to successfully get the Earth-centric XYZ coordinates of the ISS at any date and time down to the second.

However, I realized I couldn't impliment this into the PyPortal because it had limited libraries. Therefore, I switched to a Raspberry Pi. This process was initially challenging due to the new interface of the device, but after a day I was able to connect everything. I copied all of my code from the virtual environment to my Raspberry Pi, and soon I was able to display the map with the prediction line, after doing some math conversions. 

For milestone 3, I will need to upscale the image that it produces because right now it is only 400x200, which is the resolution of the PyPortal screen. Then, I plan on adding another modification, maybe something with calculating distances.

# First Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/rGwitP7QFbk?si=WOAO3podUOh1nJxD" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

For my first milestone, I was able to complete my base project. I built an International Space Station (ISS) tracking device that displays the current location of the ISS in the form of a red dot, and shows a line in yellow, representing the trail of the ISS. I used the Adafruit PyPortal to display the project and used Python on Visual Studio Code to program the display.

The biggest challenge of this process was ensuring I had up to date technology, and that I followed the instructions on the tutorial correctly. I was given an Adafruit project tutorial online and I needed to carefully read and follow the instructions. Initially all went well while I was initializing the PyPortal and downloading all of its libraries. I was able to import Circuit Python and also create a D: drive to store all of my project files. However, when I imported the code and attempted to run it, I faced an error. There was a "root_group" error that, after debugging and testing with my instructor, turned out to occur during the initialization of the PyPortal. I attempted a few methods to solve this error, removing or setting a root group, but ultimately none of those efforts worked. So I traced my steps back to the start of the tutorial, and downloaded the beta "10.0" version of Circuit Python. After going through the tutorial again, I was able to successfully display the tracker on the PyPortal. 

Reflecting on this first milestone and the challenges that I faced, I realized that I need to stay calm and be open to trying new approaches when problem solving. I could've kept doing the same thing repeatedly despite seeing no gains, but instead, I tried many different approaches and ultimately was able to get the base project to work. In the future, I hope to continue developing this project as I am excited to innovate further. I will take the problem solving skills and software setup experience from the first milestone and apply it to not only my next two milestones, but also future endeavors. 


# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

# Code
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 

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

# Bill of Materials
Here's where you'll list the parts in your project. To add more rows, just copy and paste the example rows below.
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Adafruit PyPortal - CircuitPython Powered Internet Display | What the item is used for | $54.95 | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Adafruit PyPortal Desktop Stand Enclosure Kit | What the item is used for | $9.95 | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| USB C to Micro B Cable - 1 ft 0.3 meter | What the item is used for | $2.95 | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| USB cable - USB A to Micro-B | What the item is used for | $2.95 | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| 5V 2A Switching Power Supply w/USB-A Connector | What the item is used for | $7.95 | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Raspberry Pi Model 4 4GB Starter Kit | What the item is used for | $7.95 | <a href= "https://www.amazon.com/RasTech-Raspberry-Starter-Heatsink-Screwdriver/dp/B0C8LV6VNZ/"> Link </a> |
| 5V 2A Switching Power Supply w/USB-A Connector | What the item is used for | $7.95 | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| 5V 2A Switching Power Supply w/USB-A Connector | What the item is used for | $7.95 | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| 5V 2A Switching Power Supply w/USB-A Connector | What the item is used for | $7.95 | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |


# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.
