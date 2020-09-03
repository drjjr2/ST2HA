---


---

<h2 id="introduction">Introduction</h2>
<p>My basic motivation for switching to Home Assistant stemmed from the fact that I no longer wanted to pay for my home security system. And, it turns out, that some of the components that I bought 3+ years ago as part of the system were Z-Wave which I was able to successfully move from the security system to SmartThings.<br>
But recreating an alarm system using SmartThings was not super intuitive. My original plan of reusing an old Kindle Fire 7 and installing ActionTiles and using that as my panel was not successful. I would conservatively say that 1 out of every 6 days I would walk in to see the panel say “Connecting.” So finally one morning when I went to disarm my system and it said “Connecting” I went on a quest.</p>
<h2 id="what-you-should-know">What You Should Know</h2>
<p>SmartThings, for all its faults, it pretty good at hiding the nuances of your various devices from you. For example, you may or may not have ever cared that there is a “secure” way to include Z-Wave devices and a “not secure” way. This matters because things like my garage door openers and keypad locks don’t behave well if they are not securely included. One of the reasons that ST tries to drill down the brand and/or type of devices you are adding is that they can install any workarounds that are specific to your device.<br>
And then there are other oddities. My old Kwikset locks don’t accurately report their state changes when you manually unlock and lock them. And some of my dimmers are slow to report their state changes. Things that I was blissfully unaware of when I embarked on this project.<br>
This isn’t to say that it can’t be done with HA. It’s all open source and, chances are, someone has already figured out how to fix it. But the more you need to find the custom workarounds, the more you will be diving into the architecture of Home Assistant and its various components. Which, for me, is fun. But if your significant other is complaining that the kitchen lights don’t work, well…it might not be so fun.<br>
Home Assistant and its many contributors are constantly tweaking and changing things and they have done their best to make things like adding Z-Wave devices seamless. But there’s always a catch.<br>
The bottom line is: depending on your setup, you may have to learn how to grab the latest Z-Wave config files from somewhere and how to find out where to put them on your installation.</p>
<h2 id="why-did-i-switch-to-home-assistant">Why Did I Switch to Home Assistant?</h2>
<p>Like many who are switching, I want local control (or as local as possible) for my panel and devices. Simple as that. It wasn’t to learn anything about GitHub or VMs or dust off the old Linux cobwebs. Add to that, the “new” SmartThings Home Monitor (STHM, not to be confused with the legacy Smart Home Monitor, or SHM) was not as accessible for my ActionTiles and automations. I don’t hate on the “new” SmartThings App. But it seems like they are doing away with a lot of the customizable aspects like WebCore, custom device handlers, and SmartApps.<br>
I frequent Reddit and there have been a lot of conversations about Home Assistant.</p>
<h2 id="why-am-i-using-a-vm">Why Am I Using a VM?</h2>
<p>Simply put, we couldn’t find the Raspberry Pi I bought a year or so ago in a vain attempt to build a classic video game cabinet. A flood and a hurricane later and that board was lost to the wind. I had no sooner ordered the Raspberry Pi 4 from Amazon than I stumbled across this Youtube video detailing how to install Home Assistant in a VM on a PC using Oracle VirtualBox.<br>
I’ll leave it up to you to follow the instructions there. I also set a static IP, the instructons for which are in this video.</p>
<p>My Requirements<br>
Local control of the panel (no more “connecting” screens)<br>
Alexa Integration<br>
WAF, MILAF, TSAF</p>
<h2 id="my-original-smartthings-setup">My Original SmartThings Setup</h2>
<p>My automated home has been pieced together over the years since the moment we got an Amazon Echo. This means it is a disparate selection of devices including:<br>
3 WeMo on/off switches</p>
<p>ZWave<br>
Zigbee<br>
Alexa</p>
<h2 id="credits">Credits</h2>

