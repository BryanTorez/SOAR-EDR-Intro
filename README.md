<h1>SOAR EDR Project | Intro</h1>

<p align="center">
<img src="https://snipboard.io/Cuyboe.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<h2>Description</h2>
<br />
<p align="center">
Many Security operation centers, AKA SOCS, are starting to implement some kind of SOAR, "Security", "Orchestration", "Automation", and "Response Solution", if they haven't done so already. There are many different SOAR vendors out there and it doesn't really matter which one they implement since the concepts and objectives remain the same. "Reduce repetitive tasks with automation while following a structured process", these processes are also known as, Playbooks.
<br />
<br />
<br />
<img src="https://snipboard.io/yw6QFN.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
Since many SOCs are going to be using some kind of SOAR implementation, I thought it would be a great idea to provide you with another automation project. And if you haven't seen my previous project called, the SOC Automation Project, I would recommend you go and check that out. 
<br />
<br />
<br />
<img src="https://snipboard.io/Hf1s8T.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
In that project, we used Shuffle as the sword. In this project, I'll be using Tines as the SOAR platform. You might be thinking... "Can't you just use Shuffle?" And you're right, I could, but I wanted to stress the importance that a tool, is just a tool. It doesn't matter which vendor you use because the concept is the same. In addition to Tines, I'll be using LimaCharlie, acting as my EDR endpoint detection and response. I'll also have one Windows Virtual Machine, AKA VM, in the cloud as the agent. You don't need to spin up a VM in the cloud if you don't want to. You could use any Windows machine as long as it has internet connectivity. You might have a burning question, "Well Bryan, What if I don't know how to code? And that is perfectly fine. We'll be using Chatgbt to help us if needed. As well as documentation from both Tines and LimaCharlie, that will be extremely helpful. What you'll need to be successful in this project is curiosity and patience. And when building playbooks, you'll need logic and a place to diagram your workflow. 
<br />
<br />
<br />
<img src="https://snipboard.io/KAegi3.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
In this project, we will be working together to build a detection in LimaCharlie, that will detect the tool used to recover passwords on a machine. Then, we'll send that over to Tines, which will have a playbook that we'll create. (Just FYI, Tines will call playbooks "stories", so do be aware of the terminology) but anyways the story will then send us an email, send a Slack message, and finally, ask the user if they want to isolate the machine. If the user says, "yes". LimaCharlie will then isolate the machine automatically, After going through this five-part series, you will not only gain hands-on experience working with an EDR, such as LimaCharlie, but also SOAR experience using Tines. Which I am positive will help you in your professional career.
<br />
<br />
<br />
<img src="https://snipboard.io/WkdAEH.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
Now this is going to be very hands-on and can be difficult depending on your level of experience, so do plan to carve out some time if you want to participate. By the end of the project, you will have a custom detection rule built in LimaCharlie and a playbook that integrates Slack and emails, along with a responsive capability, thanks to Lima Charlie. 
<br />
<br />
<br />
<img src="https://snipboard.io/6xTEQ7.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
Beginning with part one, we will begin designing our playbook workflow, and then drawing out how we want that to work. Do keep in mind that changes can and will likely happen, as it is perfectly normal during the Playbook creation phase to find out that certain functionality, just doesn't exist, or the logic, just doesn't make sense. In other words, you don't need to know "exactly" what your playbook workflow will look like, but it is a good idea to diagram the things that you want to do, as this will help you organize your thoughts.
<br />
<br />
<br />
<img src="https://snipboard.io/moJ8Qa.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
In part two, I will walk you through on how to set up LimaCharlie and we start to get our data in from our Windows machine. 
<br />
<br />
<br />
<img src="https://snipboard.io/C2qdj4.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
For part three, you'll generate events on your Windows machine using the password recovery tool and I'll walk you through on how you can create your own custom detection and response rule in LimaCharlie. This rule is then going to be sent over to Tines to begin our automation.
<br />
<br />
<br />
<img src="https://snipboard.io/Eaz4yR.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
In part four, you'll get set up with Slack, which is a messaging platform, and Tines. The objective for this part is to begin integrating LimaCharlie with Tines. Essentially, creating that link between the two applications, and then we'll validate to make sure that we are getting the detections inside of Tines. 
<br />
<br />
<br />
<img src="https://snipboard.io/mixHth.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
Finally, the last part of the project will be all about automation. This is where we begin creating our playbook/story in Tines.
<br />
<br />
<br />
<img src="https://snipboard.io/kFfxec.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
I hope that once you go through this project, not only will you learn something new, but also gain more confidence in your technical skills. One thing I do want you to keep in mind is that if you do encounter errors please try and research them and see what you can find. Go through documentation and utilize Chatgbt.
<br />
<br />
<br />
<img src="https://snipboard.io/36pmJL.jpg" height="100%" width="100%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
I hope that you're as excited as I am to get started on this project. If you do plan on following along, please think about putting it into your portfolio on GitHub. I really want you to showcase your work and be proud of something that you built. That is it for this intro and thank you for reading. Remember to stay curious and do things differently.
<br />
<br />
<br />
