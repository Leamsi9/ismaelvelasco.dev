## Tech debt: the good, the bad and the costly

Today we take a deep dive into technical debt: what is it, when is it good, when is it terrible, how to measure it, how to cost it, how to address it.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1658365848019/lXG6VHiRN.png align="left")

You may have noticed I added a [new Tech Talks section](https://ismaelvelasco.dev/tech-talks) (OK, no way you noticed). It has 15 recordings from meetups, conferences and even COP26. I will periodically introduce one here. I decided to start with my talk on Technical Debt, because I have been selected to give a [1 day workshop on the subject](https://conferences.isaqb.org/software-architecture-gathering/full-program/#advanced-technical-debt-management-the-good-the-bad-and-the-costly) in November, at one of the world's [leading architecture conferences](https://conferences.isaqb.org/software-architecture-gathering/), by the [International Standard in Training and Certification of Software Architects]((https://isaqb.org/)) - probably the world's foremost software architecture certification body. It is a genuine honour. 

<h2>So what is tech debt?</h2>

Very often, tech debt is defined as a conscious trade off of quality for speed, or a result of poor design decisions. But while both of those are good examples of tech debt, tech debt can also come to absolutely top quality code: if it fails to evolve with the tech ecosystem. The cutting edge app of 2010 is very often the creaky, slow and plainful monolith of in 2020. It's not that the original choices were suboptimal: it's that time moves fast in tech, and code needs to constantly evolve to keep in sync.


<h2>Technical Debt Accounting Framework</h2>

Not all technical debt is created equal. Below is a framework you may find useful in mapping different parts of your application:

<h3>Low Interest Technical Debt</h3>

Technical debt, like financial debt, can be useful, helping you enter the market and gain traction with an MVP, or allowing you to innovate, or rebuild. That's when your debt is "low interest", you understand the trade offs and the pain is in your future, with a plan to pay it back before it gets painful.

<h3>High Interest Technical Debt</h3>

High interest debt, that's risky, and much harder to pay off. Here your technical pain is not ahead but right now, and if you're nor careful, it will compound into a debt default. Technical debt now places serious operational and commercial constraints on the entire company, and creates reputational risks, from security breaches to service interruption.

<h3>Technical Debt Default</h3>

This is where your company is at existential risk because of technical debt. Your core platforms may have passed End Of Life and with widely publicised critical exploits, and you advertise this in your website headers. Your system has become so bloated and is so highly coupled that no one really knows what everything does, and everyone is afraid to change things because every change creates side-effects. Your new features grind to a halt, your devs leave, your company stagnates and loses users to more reliable competitors.

So how do you rigorously measure technical debt? How do you know which specific classes are most tightly coupled or more likely to create side effects or most difficult to understand? How do you measure the impact, as opposed to the presence of technical debt on your team or company's feature development process? How do you estimate its financial cost? How do you choose which areas of the code to refactor first? How do you know when replacement is the only option?  How do you persuade the business of the need to invest in technical debt?

%[https://youtu.be/McO_ONKxwNU]

The talk above offers answers to these questions, and the online workshop will actually train you to apply them in practice.  If you enjoy the talk, you might want to [sign up](https://conferences.isaqb.org/software-architecture-gathering/tickets/) for the (online) workshop. Do share any feedback or suggestions for things I should clarify or add ahead of the course!
