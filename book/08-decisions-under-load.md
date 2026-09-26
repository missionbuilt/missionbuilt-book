# 8. Decisions Are Made Under Load

## Stress Tests the System

> *Stress doesn't break the system. It exposes what was already weak.*

In the gym, testing under load is a simple idea. Your ability to move weight when you're tired is the real signal of progress, and every lifter knows it. The same test exists in product leadership, systems design, and incident response, but most of us don't run it until the moment runs it for us.

The Log4j vulnerability in December 2021 made that brutally clear. A zero-day exploit in a widely used Java library allowed remote code execution with minimal effort, and suddenly nearly every organization was asking the same urgent questions:

- Are we exposed?
- Where is Log4j deployed in our environment?
- Do we have visibility into historical access or exploitation attempts?

This was never just a code issue. It was a test of organizational readiness, technical, operational, and strategic all at once. Teams that had practiced incident response, mapped their architecture, and built cross-functional trust could move with purpose. Others stumbled, not because they didn't care, but because they had never trained for the moment.

It was the backup problem, writ large. Many companies back up data religiously, but few test whether they can actually recover it. Fewer still know how long recovery will take, or what their RTO (Recovery Time Objective) or RPO (Recovery Point Objective) really are. The lesson gets learned the hard way, and it is always the same one: backups are only as valuable as your ability to restore fast.

Log4j forced a parallel reckoning. Malicious scanning began months before the public disclosure, but most organizations didn't retain accessible data that far back. They had cold storage, frozen or tiered off to save money, but they had never practiced bringing it back online quickly for an investigation. When the pressure hit, teams had to figure out, often in real time, how to thaw data, rehydrate logs, and search for infection markers across old records.

Some had tested this process before. They knew the commands, the timing, the quirks of their tooling, and they had trained like operators. Others hadn't. Some couldn't search more than 30 days back, and others found that recovering historical logs was so cumbersome it may as well not have existed. Those companies weren't just missing data, they were missing a disaster recovery plan for threat analytics.

At Elastic, the customers who had previously rehearsed these data flows, archiving, restoring, and hunting, were able to quickly triage and verify impact, drawing from months-old telemetry. They weren't just ingesting logs, they were building institutional memory.

That mirrors what elite military units do when they train decision-making under fatigue. In Navy SEAL training or Army Special Forces SERE programs, candidates are made to perform operational tasks after sleep deprivation, cold water exposure, and physical exhaustion, not to break them but to reveal what is already broken. In those moments you don't rise to the level of the manual, you fall to the level of your defaults, and the only way to improve those defaults is to train them, deliberately, under controlled stress.

The industry has lived the same shape since. In February 2024, the Change Healthcare ransomware attack took down claims processing, prescription routing, and billing across most of U.S. healthcare. The vulnerability wasn't novel, but the organizational readiness was. Hospitals that had drilled their incident response could keep dispensing prescriptions on paper, while others lost weeks to manual workarounds because no one had practiced operating without the platform. Same lesson, different load. Stress finds the truth.

### The 2026 Stress Test Is Machine-Speed

The Log4j-shaped stress test was bad. The 2026 version is worse, because the attackers are no longer moving at human speed.

The mean time from vulnerability disclosure to confirmed exploitation has fallen from 2.3 years in 2019 to under one day in 2026. Breakout times, the window between initial compromise and lateral movement, are measured in seconds. Phishing campaigns crafted by large language models hit click-through rates 4.5 times higher than human-written ones, and capabilities that once required nation-state expertise are now available to anyone with an API key.

If you are not using AI to battle AI, you will lose. Defensive AI is the new minimum entry fee just to stay level. There is a whole chapter on AI later in this book, and this is a big part of why it needed one.

### Stress Finds the Truth

The same test runs in product and platform work. You might have a dashboard for monitoring, a workflow for restores, and a playbook for incident response, but unless you've tested them when it matters, they're just ideas. Stress finds the truth.

So whether you're squatting on trembling legs after five working sets or trying to rehydrate petabytes of logs to confirm an intrusion, the system only works if it works under pressure. This isn't a new idea. I brought it up in Chapter 2 with James Clear's line:

> *"You do not rise to the level of your goals. You fall to the level of your systems."*

Under the weight of stress and urgency, that line deepens. Goals vanish in a crisis and roadmaps collapse under pressure, and what remains is the infrastructure you've trained, tested, and trusted. Whether that's a disaster recovery pipeline, a muscle memory forged in fatigue, or a culture that knows how to move without waiting for permission, it's your system that carries you. Resilience is not something you react your way into, you build it, deliberately, daily, and under load.

---

## Clarity Beats Certainty

> *You don't need to know the outcome to know how to act.*

There's a myth in leadership, and in lifting, that success comes from always having the right answer, that if you just gather enough data, wait long enough, or plan hard enough, certainty will arrive and carry you through. The best teams, the best lifters, and the best products I have seen don't run on certainty, they run on clarity.

You see it in moments of disruption. In early 2020, when the COVID-19 pandemic rewrote every assumption about business, teams that waited for complete information froze. The ones who moved quickly didn't do it recklessly, they did it with intention.

- **Zoom** opened up free access to educators worldwide. Daily meeting participants skyrocketed from 10 million in December 2019 to 300 million by April 2020.
- **Peloton** overhauled its entire supply chain when demand outpaced capacity. By Q4 2020 it reported 232% year-over-year revenue growth and added over 1 million new subscribers.
- **Notion** refocused messaging for the remote work moment. Its user base grew from 1 million to over 4 million in 2020.

None of them knew how long the shift would last, but they had clarity of mission, and that clarity became a compass.

It's the same clarity high-level lifters use when they train with RPE (Rate of Perceived Exertion). Instead of sticking to a fixed number on the bar, they assess how each set feels in real time. On some days that means pulling back to preserve recovery, and on others it means pushing heavier than planned. None of that is guesswork. It's informed adaptation, which is what clarity looks like in action when the conditions keep changing.

This is where the OODA Loop earns its place. We met it in Chapter 1: Observe, Orient, Decide, Act. The point isn't perfection, it's momentum, and you act, assess, and adjust faster than the environment can overwhelm you. The model applies just as well to product releases, user feedback, platform incidents, and organizational change as it does to military operations. You're not waiting for every signal to align. You're moving with awareness, grounded in your principles, and fast enough to respond before inertia sets in. That is where clarity beats certainty, and it's why you don't always need a perfect map if you've trained your compass.

Let's be honest: Agile is a loaded word. Some teams swear by it, others roll their eyes, and more often than not the problem is with the implementation rather than the philosophy. Too many teams have had Agile forced on them by someone who read a textbook but never wrote a line of code. The rituals become rigid, the flexibility becomes performative, and the spirit gets lost in the ceremony.

I'm a firm believer in the Agile mindset, but not the dogmatic, by-the-book version. True agility means responding quickly to new information and iterating with intent, and that only works if the team has clarity. Without it, Agile devolves into a flurry of half-finished tickets, context switches, and directionless pivots. The point was never to abandon focus. The point was to stay mission-aligned, laser-focused on the *"why,"* while remaining flexible on the *"how."*

Where I most often see Agile fail is when it becomes a cover for indecision, when teams confuse agility with ambiguity, and when the lack of a clear goal gets labeled as *"keeping our options open."* I also see it fail when people demand certainty before committing to action. Even today, with more data than ever before, certainty is rare. We have telemetry, user interviews, funnel analysis, Salesforce records, and analyst feedback, and the decision on what to build next is still more art than science. If there was a playbook to follow, we'd be project managers. But we're product managers. Our craft isn't perfect foresight. It's translating user pain into progress, surfacing the *"why"* beneath the *"what,"* and seeing the pattern behind the request.

As Nathaniel Fick wrote in *One Bullet Away*, his memoir about the transformation from Ivy League student to Marine officer leading combat missions in Afghanistan and Iraq:

> *"Complex ideas must be made simple, or they'll remain ideas and never be put into action."*

That's our job. We take everything we know, the signals, the inputs, the intuition, and turn it into action, not after a perfect analysis and not when every detail is known, but when it's time to move. We do that not by being certain but by being clear: clear on the mission, clear on the user, and clear on what matters most right now. In the fog of delivery, feedback, and shifting priorities, the job is not to predict perfectly, it's to steer on purpose. Certainty asks, *"Are we sure?"* Clarity says, *"Here's what we do next."*

---

## Training for Chaos

> *We don't rise to the level of our plans. We fall to the level of our preparation.*

In the last chapter I talked about training the engine, building general physical and mental capacity rather than just specific skills. That alone isn't enough, though. What happens when the plan vanishes, when you're under pressure, short on time, and forced to act without hesitation? That's when preparation has to become instinct.

I learned this firsthand as a U.S. Army paratrooper. Before you ever board a plane, you train on the ground for weeks, drilling every movement until it's embedded: how to hook up your static line, how to check your gear, how to exit, how to land. You jump from towers, you simulate the aircraft, and you practice failure, not because you want it, but because it's coming.

> *You want to fail when you're four feet off the ground, not 800.*

We don't take our first flight until the basics are second nature, because stepping out the side door of a C-130 at 800 feet, in pitch black, is against every self-preservation instinct you have. In that moment you don't want to be thinking through a checklist. You want to be moving. If your main chute doesn't deploy, you have 9 to 10 seconds to respond before impact, and there is no time to think in that window. You just act.

I still remember my first jump: the roar of the engines, the rush of the open door, and then standing up, hooking up, and waiting for the green light. I didn't feel fear and I didn't feel stress. I felt clarity. I knew what to do and I executed, because we had trained for it.

That same mindset exists in the best teams, even in tech. At Netflix, Chaos Monkey was built to deliberately shut down random services in production, so that both the systems and the people would learn to adapt under pressure. They didn't just hope their systems were resilient, they trained them to be, and the results were measurable. Netflix prevented 80% of potential outages through the learnings surfaced by Chaos Monkey and the broader chaos engineering discipline. These weren't hypothetical flaws. They were real vulnerabilities, caught early because someone had the courage to test failure on purpose. That wasn't sabotage, it was preparation. You don't find out whether you're ready in the middle of a real incident, you find out beforehand, if you're willing to simulate the storm.

You see this in sport, too. During the CrossFit Open, athletes receive surprise workouts announced just days before competition. Movement patterns shift, equipment combinations vary, and sometimes it's a short, explosive sprint while other times it's a long, grinding engine test. You don't know what's coming, and that's the point. The unpredictability isn't accidental. It reflects one of CrossFit's founding principles: prepare for the unknown and the unknowable. In real life, just like in combat, product development, or incident response, you don't get a playbook with advance notice. You're asked to perform under pressure, with incomplete information and limited control.

By designing chaos into the format, new standards, awkward movement pairings, strange pacing demands, CrossFit forces athletes to confront not just their physical readiness but their emotional and mental adaptability. The top performers aren't just strong, and they don't just move well. They stay composed when the plan disappears. That's the test, and that's the transferability. The Open doesn't only reward fitness. It rewards clarity under fatigue, pacing under uncertainty, and strategy when the rules shift. The chaos is the feature, not a bug, and it reveals what structure alone can't.

This belongs in the same category as paratrooper training or chaos engineering. You don't need bullets or breakage for chaos to be real, all you need is volatility, pressure, and a demand for action. When that moment comes, the best don't panic. They breathe, they move, and they decide.

I want to pause here and share something personal. I've never claimed to have done the hardest thing in the military. Many others have faced more direct danger, made life-or-death decisions in the field, and carried far heavier loads, and Nate Fick, whose story I referenced earlier, is one of many. But I've also learned that you can't live your life comparing hardships. Chaos shows up in many forms, and every one of us has moments when our training is tested by stress.

For me, that came during my deployments in support of Operation Enduring Freedom and Operation Iraqi Freedom, where I served as an intelligence analyst in two Combined Air Operations Centers, first at Prince Sultan Air Base in Saudi Arabia and then at Al Udeid Air Base in Qatar. My job was to represent U.S. Army interests in daily joint targeting and mission planning, to advocate for the air support our soldiers needed downrange. That meant walking into rooms where I was often the lowest-ranking person present, trying to secure limited airframes for missions that couldn't afford to fail. There were more missions than aircraft. Everyone in the room wanted to help, but everyone had missions to support. The real pressure wasn't the data. It was the conversation, the negotiation, the weight of knowing that if I couldn't make our case clearly, the soldiers downrange might not get the support they needed.

That stress taught me the true value of clarity, not just in numbers but in stories. It wasn't the PowerPoint or the packet that made the difference. It was being able to explain why this mattered, what the risk really was, and who would be impacted if we didn't act. I learned young, and under pressure, how to speak across rank and service, how to translate intelligence into insight, and most importantly, how to give a shit, loudly, clearly, and with purpose.

I didn't have a name for the motto then. As I shared in the prologue, the words live on the patch of VMM-364, the Purple Foxes, and I would learn the squadron's history later in my career. But under the load of those rooms in the CAOCs, the principle was already running the work.

One of the awards I received, the Army Commendation Medal, noted that I served in multiple roles normally held by ranks far above mine, including as the BCD Intelligence NCOIC (a Sergeant First Class role) and as an Intelligence Plans Officer, a position typically held by a Major. I don't say that to boast. I say it to underscore this: you don't perform under stress unless you care deeply about the mission and the people it impacts.

That lesson stayed with me in uniform, in product, and in leadership. It's not process that drives you when the pressure hits. It's principle, it's preparation, and it's the ability to act with conviction because you know exactly what's at stake. You don't have to be on the front lines to know what chaos feels like. You just have to care enough to move when it matters most.

---



