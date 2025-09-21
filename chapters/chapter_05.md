# Chapter 5

Michael's day started at 6:15 AM with his phone buzzing on the nightstand. A production alert from the monitoring system he'd built two years ago, back when he still wrote code more than he attended meetings about writing code.

Database connection pool exhausted. He knew the fix—increase the pool size and restart the service—but he also knew that fixing it himself would undermine the on-call rotation he'd spent six months establishing. 

He sent a message to the on-call engineer instead: "Seeing the DB pool alert. Let me know if you need anything."

The response came back in three minutes: "Already on it. Increasing pool size now."

Michael smiled despite the early hour. His team was good. They knew their stuff, they helped each other, and they rarely needed him to solve technical problems anymore. Which was exactly what he'd wanted when he'd taken the promotion to Technical Lead three years ago.

What he hadn't anticipated was spending most of his time protecting them from people who had no idea what they did.

His wife Kate was already awake, getting ready for her shift at the hospital. She was an ER nurse, which meant she dealt with actual emergencies involving real consequences, not the manufactured urgency of quarterly planning sessions and strategic realignment initiatives.

"Another production issue?" she asked, watching him check his phone.

"Already handled. The team's got it."

"Good team."

"The best."

Kate had heard enough of his work stories to understand the basic dynamics: he had smart people who did important work, and he spent his days in meetings with people who didn't understand either the smartness or the importance.

"What time will you be home?" she asked.

Michael checked his calendar. Back-to-back meetings until 6 PM, then the quarterly planning session that Vincent had moved to 7 PM because it was the only time that worked with his schedule.

"Late. Probably 9."

Kate nodded. She'd stopped asking why his meetings ran so long, just like he'd stopped trying to explain that most of them could be emails, if anyone actually read emails anymore.

"Jake has soccer practice at 4. I can pick him up if you can't make it."

"I'll try to duck out early."

"It's fine, Michael. He knows you're busy."

That was the problem. Jake was twelve, and he was already learning that work came first, meetings were more important than soccer games, and adults spent their evenings on laptops instead of helping with homework.

Michael kissed Kate goodbye and headed to ByteSauce, where his first meeting was with Vincent about the Taskly migration timeline. Vincent wanted to know why the engineering teams were "resistant to change" and what Michael could do to "drive adoption."

"The teams aren't resistant to change," Michael explained for the third time in two weeks. "They're resistant to tools that don't work as well as the tools they're already using."

Vincent consulted his notes. "But the Innovation Lab has assured me that Taskly has all the features we need."

"It has some of the features we need. The API doesn't exist yet, bulk operations are limited, and the migration tools have data integrity issues."

"Those sound like implementation details. Can't the teams work around those limitations?"

Michael stared at Vincent across the conference table. "The limitations aren't edge cases. They're core functionality gaps that affect daily workflows."

"Right, but from a strategic perspective, we need to show progress on internal tool adoption. The board is expecting metrics."

Michael had learned to recognize this moment in conversations with Vincent: the point where technical reality collided with executive expectations, and reality was expected to yield.

"What kind of metrics are you looking for?" he asked.

"User adoption rates, productivity improvements, cost savings. The usual KPIs for digital transformation initiatives."

Michael opened his laptop and pulled up a spreadsheet he'd been dreading. "Here's what I can give you. We can migrate the teams to Taskly and show 100% adoption within two weeks."

Vincent brightened. "That's exactly what I want to hear."

"But," Michael continued, "productivity will drop by approximately 30% for the first month while people learn the new system, and it'll stay 15% below baseline until the missing features are implemented."

Vincent's enthusiasm dimmed. "Can we quantify the long-term benefits to offset the short-term productivity loss?"

"What long-term benefits?"

"Reduced vendor costs, improved collaboration, better visibility into project status."

Michael consulted his spreadsheet. "We'll save $50,000 annually on licensing fees. Collaboration might improve once the API is built, but that's Q2 at the earliest. Visibility will actually decrease because Taskly's reporting is less flexible than what we currently have."

Vincent made notes. "So we're looking at short-term pain for long-term gain."

"We're looking at short-term pain for minimal long-term gain, assuming the Innovation Lab delivers on their roadmap promises."

"But you can make it work?"

Michael recognized another moment: the point where his job required him to say yes to something he knew was a bad idea.

"We can make it work," he said.

After the meeting, Michael walked back to his desk feeling like he'd just agreed to perform surgery with a butter knife. Technically possible, but unnecessarily difficult and likely to cause more problems than it solved.

His team was clustered around Alex's monitor, looking at something that was making them all shake their heads.

"What's the crisis?" he asked.

Alex pointed to her screen. "Taskly's data export function. It generates CSV files, but they're not actually comma-separated. They're semicolon-separated, and the encoding is wrong, so any non-ASCII characters get corrupted."

Mack laughed. "It's not CSV, it's SSV. Semicolon-Separated Values. Revolutionary."

Jordan looked up from his laptop. "I've been trying to get clarification from the Innovation Lab, but they keep saying it's a 'configuration issue' that can be resolved through 'user training.'"

Michael sat down at his desk and opened his email. Seventeen new messages since the meeting with Vincent, including three from the Innovation Lab asking for "feedback on the user experience" and two from other team leads reporting similar problems with the migration process.

He started typing a response to the Innovation Lab, explaining the technical issues his team had identified. Halfway through, he deleted it and started over. The second draft was more diplomatic but still honest about the problems. He deleted that one too and wrote a third version that focused on "opportunities for improvement" and "collaborative problem-solving."

He sent the diplomatic version and immediately felt like he'd betrayed his own team.

His phone rang. Kate, calling from the hospital.

"Quick question," she said. "Jake's science fair project is due tomorrow, and he's panicking about his volcano. Can you stop by the store and get baking soda and food coloring?"

Michael looked at his calendar. The vendor review meeting at 3, the budget discussion at 4:30, the quarterly planning session at 7.

"What time does the store close?"

"Nine, I think. But he really wants to practice the presentation tonight."

"I'll figure something out."

He hung up and immediately sent a message to his team: "Can someone cover the vendor meeting for me? Family emergency."

Alex responded first: "I can handle it. Everything okay?"

"Twelve-year-old science fair crisis. Nothing life-threatening."

"The worst kind of emergency," Mack replied. "Good luck with the volcano."

Michael left the office at 2:30 and drove to Target, where he bought baking soda, food coloring, and a poster board that Jake had forgotten he needed. By the time he got home, it was 4 PM, and Jake was sitting at the kitchen table surrounded by textbooks and looking overwhelmed.

"Dad! I can't get the chemical equation right, and the volcano looks terrible."

Michael sat down next to him and looked at the clay volcano he'd built. It was lopsided and painted in colors that didn't exist in nature, but it was clearly the work of someone who'd put effort into the project.

"It looks like a volcano to me," he said. "What's the chemical equation supposed to show?"

"The reaction between sodium bicarbonate and acetic acid. But I don't understand why it makes carbon dioxide."

Michael grabbed a piece of paper and started drawing molecular diagrams. For the next hour, he explained chemical reactions, helped Jake practice his presentation, and watched his volcano erupt three times with increasing enthusiasm.

It was the best hour of his day.

At 6 PM, his phone started buzzing with messages from the quarterly planning session. Vincent wanted to know where he was, the budget numbers needed clarification, and someone had questions about the Taskly timeline that only he could answer.

"I have to take a work call," he told Jake.

"But we haven't finished the poster."

"Your mom can help with the poster. This will just take a few minutes."

Michael spent the next ninety minutes on a conference call, explaining why the engineering budget couldn't be cut by 20% without affecting project timelines, why the Taskly migration would impact productivity, and why the Innovation Lab's optimistic delivery dates were probably unrealistic.

By the time he hung up, Jake had gone to bed, and Kate was finishing the science fair poster at the kitchen table.

"How'd the call go?" she asked.

"Same as always. Everyone wants everything faster and cheaper, and no one wants to hear why that's not possible."

Kate held up the poster. "Think this will work?"

Michael looked at Jake's project: a carefully researched explanation of chemical reactions, illustrated with diagrams he'd helped him draw, and a volcano that would definitely erupt when he demonstrated it tomorrow.

"It's perfect," he said.

"He was excited that you helped with the chemistry part. He said you made it make sense."

Michael felt a familiar tension between pride and guilt. He was good at explaining technical concepts, solving complex problems, and helping people understand difficult ideas. But he spent most of his time in meetings where those skills were irrelevant, talking about timelines and budgets instead of the actual work.

"How was your day?" he asked.

"Three heart attacks, two overdoses, and a kid who broke his arm falling off his bike. Standard Tuesday in the ER."

Michael nodded. Kate dealt with real problems that had clear solutions: stabilize the patient, treat the symptoms, save the life. His problems were abstract and political: balance competing priorities, manage expectations, translate between technical reality and business requirements.

"Do you ever think about what you'd be doing if you weren't managing people?" Kate asked.

"Every day."

"What would you be doing?"

Michael thought about the production alert that morning, the satisfaction of identifying a problem and implementing a solution. "Writing code. Solving technical problems. Building things that work."

"Why don't you go back to that?"

"Because someone has to protect the people who are writing code and solving technical problems. If I don't do it, they'll get someone who doesn't understand the work."

Kate finished cleaning up Emma's art supplies. "So you're sacrificing your career satisfaction to protect your team's career satisfaction."

"Something like that."

"That's very noble. Also probably unsustainable."

Michael's laptop was open on the counter, showing seventeen new emails from the evening's planning session. Action items, follow-ups, and requests for more detailed analysis of problems he'd already explained three times on the call.

"I should probably respond to these," he said.

"Jake's presentation is at 10 AM tomorrow. Think you can make it?"

Michael opened his calendar. The Innovation Lab retrospective at 9:30, the vendor contract review at 11, and the all-hands meeting at 2.

"I'll try to move the 9:30."

"He'd really like you to be there."

"I know. I'll make it work."

Kate went upstairs, and Michael sat at the kitchen table with his laptop, responding to emails about strategic initiatives and budget reallocations. Outside, he could see the lights in the office building across the street, where other people were probably having similar conversations about impossible timelines and competing priorities.

His phone buzzed with a text from Alex: "Vendor meeting went fine. They agreed to extend the contract terms. Nothing urgent."

Michael typed back: "Thanks for covering. How bad was it?"

"Standard vendor meeting. They want more money, we want better service, everyone agreed to think about it."

"Appreciate you handling it."

"No problem. Family stuff okay?"

Michael looked at Jake's science fair poster, propped up against the counter and ready for tomorrow's presentation. "Yeah. All good."

He closed his laptop and went upstairs, where Kate was already asleep and Jake's bedroom light was still on. He knocked softly on his door.

"Dad?" he called.

"Just wanted to say good luck tomorrow. Your volcano is going to be great."

"Will you be there?"

"I'll be there."

Michael turned off his phone and set it on the dresser. Tomorrow's problems could wait until tomorrow.
