---


---

<h2 id="what-you-should-know">What You Should Know</h2>
<p>SmartThings, for all its faults, it pretty good at hiding the nuances of your various devices from you. For example, you may or may not have ever cared that there is a “secure” way to include Z-Wave devices and a “not secure” way. This matters because things like my garage door openers and keypad locks don’t behave well if they are not securely included. One of the reasons that ST tries to drill down the brand and/or type of devices you are adding is that they can install any workarounds that are specific to your device.<br>
And then there are other oddities. My old Kwikset locks don’t accurately report their state changes when you manually unlock and lock them. And some of my dimmers are slow to report their state changes. Things that I was blissfully unaware of when I embarked on this project.<br>
This isn’t to say that it can’t be done with HA. It’s all open source and, chances are, someone has already figured out how to fix it. But the more you need to find the custom workarounds, the more you will be diving into the architecture of Home Assistant and its various components. Which, for me, is fun. But if your significant other is complaining that the kitchen lights don’t work, well…it might not be so fun.<br>
Home Assistant and its many contributors are constantly tweaking and changing things and they have done their best to make things like adding Z-Wave devices seamless. But there’s always a catch.<br>
The bottom line is: depending on your setup, you may have to learn how to grab the latest Z-Wave config files from somewhere and how to find out where to put them on your installation to make things work the way they “used to.”</p>

