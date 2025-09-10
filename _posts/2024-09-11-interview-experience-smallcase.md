---
title: "Interview experience at Smallcase"
date: "2025-09-10  12:06:00"
author: VIVEK_0001
---

I applied for this Backend Intern role at [Smallcase](https://www.smallcase.com) via LinkedIn jobs.

## Round 1: Telephonic HR Round

After a few weeks of applying, I received a call from the smallcase that my application was shortlisted. He briefed me about the next steps, a technical round, while asking about my current commitments, notice periods, and availability if selected. He then scheduled the technical interview call.

## Round 2: Technical Round

This round started with discussions about my projects and previous work experience. Then there were questions about NestJS, like what are the features of NestJS, followed by a few questions on MongoDB and PostgreSQL. There were also some systems questions such as how to optimize read and write operations in both SQL and NoSQL databases, and questions about TypeScript, specifically generic types. I also got an easy challenge to create a generic interface schema in TypeScript for different job types (‘email’, ‘push’, ‘whatsapp’) with channel specific payload definitions on a shared google docs. We wrapped up with feedback from this call. After the interview ended, 3-4 hours later I got a call from Smallcase saying I had made it to the next round.

## Round 3: Live Coding Round

After around four weeks, I got a slot for the second technical round. It started with introductions from both sides, and then the interviewers shared a three-page document containing a problem statement. The challenge was to build a clean, scalable backend system for a portfolio tracker from scratch within one hour on a live call with screen sharing.

There were some rules for this round. I was not allowed to use AI tools, only official documentation. Using a database was optional; file-based storage was also allowed. There were three use cases that had to be solved, and missing even one of them would mean instant elimination. The interviewer also mentioned that previous interviewees had tried building a backend system, but by the end of the time their solutions were not fully completed. He warned me that no matter how scalable the architecture was, if at the end of the timer I missed even one of the three use cases, I would be eliminated instantly. I was also given the option to just write functions in any tech stack for the use cases if I wasn’t comfortable building a full backend system.

But I decided to take the toughest path and build APIs for these use cases using MongoDB as the database and a Node + Express server with TypeScript for the backend. I chose this path not only because I enjoy taking risks and working under pressure but also because I was confident that I could build this system within one hour without AI. I first designed the schema and endpoints on paper, then started coding. Throughout the process, I clarified my doubts with the interviewer, and he was very supportive, addressing even the smallest questions.

The sad part was that I was not able to complete all the use cases within the given one hour, but I doesn't mean that I gave up. I requested an extension of five more minutes, and within the next 5–6 minutes, I pulled it off. Then the evaluation of the system began. I had to demonstrate the system to show that it fulfilled all the challenges. I was able to solve all three of them, but there was one misunderstanding. I had misinterpreted the type field of a holding. It was supposed to be “buy” or “sell,” but I thought it as  `intraday`, `options` or other types. The actual requirement was simple: if `type == buy`, then use `+=`, else if `type == buy`, then use `-=`. I explained this mistake during the evaluation, apologized, and also explained how I would fix it.

During further evaluation, we noticed another bug. When a stock, say TCS, was purchased and it already existed in my portfolio, instead of just only updating the average price and shares, my system was also adding a new holding. At this point, I started worrying, but I quickly looked into the code and instantly noticed that I had forgotten a `return` statement inside an `if-block`, which was causing both conditions to execute. Other than that, everything was working as expected and also the system architecture was solid. If you’re curious, here’s the [GitHub repo](https://github.com/vivektripaathi/smallcase-portfolio-tracker) of the solution I built during this live coding round.

We wrapped up this round with feedback. A few hours later, just like the previous round, I got a call from Smallcase saying I had cleared this round too. They also shared the positive feedback the interviewer had given about me and scheduled the slot for the last round.

## Round 4: Final Cultural Fit Round

This round started with introductions from both sides. It was more of a two-way, casual conversation. I talked about my previous work, my expertise, and the projects I had done. Then I asked some curious questions about Smallcase, like what teams and products they have, and which team I would be working with. We also discussed my college, availability, and current commitments. There were a few general questions like what I would bring to the team as an intern, what kind of culture I was looking for, and what kind of culture Smallcase had. Overall, it was more about alignment and fit rather than technical skills.

## Final Verdict

On the same day as the last round, I got the call: I was selected and offered the Backend Intern role at Smallcase! We discussed joining dates and next steps, and I’m thrilled to share that I accepted the offer. On the same day of the cultural fit round, I got a call from Smallcase. They told me that I had been selected and we discussed things like the earliest date I could join and when I would receive the offer. As per the discussion, I received the official offer for the Backend Intern role at Smallcase 🥳.
