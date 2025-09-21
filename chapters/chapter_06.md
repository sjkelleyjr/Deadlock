# Chapter 6

The conference room had been transformed overnight. Someone had taped index cards to the walls, arranged sticky notes in colorful columns, and positioned a flip chart next to the whiteboard. A stack of planning poker cards sat in the center of the table like a deck waiting for a game nobody wanted to play.

Sarah stood at the front of the room with the enthusiasm of someone who'd spent the weekend watching agile methodology videos on YouTube.

"Good morning, everyone! Today we're going to revolutionize how we approach sprint planning. No more guessing about timelines or scope creep derailing our deliverables."

Alex slid into her usual back-corner seat and surveyed the room. The walls were covered with user stories written in Sarah's neat handwriting: "As a user, I want to export my data so that I can analyze it offline." "As a user, I want to integrate with third-party APIs so that I can streamline my workflow."

Mack arrived with his coffee and stopped short when he saw the index card installation. "Did we get acquired by a startup while I was getting coffee?"

"We're implementing proper agile practices," Sarah announced. "I've been working with a consultant to redesign our planning process."

Jordan took a seat in the middle of the room where he could see everyone's reactions. "This looks comprehensive. Walk us through the new approach."

Sarah consulted her notes, which were organized in what appeared to be a color-coded system. "We're going to estimate each user story using story points, then commit to a realistic sprint velocity based on our team's capacity."

Michael looked up from his laptop. "How do we determine story points for features we've never built before?"

"Great question. We'll use planning poker to reach consensus on complexity." Sarah held up the deck of cards. "Everyone gets cards with Fibonacci numbers. We estimate the effort relative to our baseline stories."

Alex examined the user stories on the wall. Most of them were variations of "integrate with external system X" or "implement compliance requirement Y." The kind of work that sounded simple until you discovered the external system's API was documented in broken English and the compliance requirement had seventeen sub-requirements that contradicted each other.

"What's our baseline?" Mack asked.

Sarah pointed to an index card labeled "User Login." "This is our 1-point story. Simple, well-defined, minimal complexity."

Alex studied the login story. It looked simple on the card, but she remembered implementing it. Two weeks of OAuth integration, password policy compliance, and multi-factor authentication requirements that hadn't been mentioned in the original specification.

"And this?" Jordan pointed to a card labeled "Third-party API Integration."

"That's what we need to estimate today. Along with CSV export functionality, data migration tools, and the new reporting dashboard."

Mack leaned back in his chair. "CSV export is the Rube Goldberg machine we talked about last month. The one that requires five microservices and a compliance framework."

"Right, but now we can break it down into smaller, manageable pieces."

Alex looked at the CSV export card, which simply read: "As a user, I want to export my data to CSV so that I can analyze it in Excel." No mention of the legal requirements, the encryption pipeline, or the approval workflow that had turned a simple feature into a six-month project.

"Let's start with the API integration," Sarah said, distributing planning poker cards to everyone. "Remember, we're estimating complexity relative to the login story. Everyone ready?"

Michael held his cards like he was playing actual poker and losing. "Which API are we integrating with?"

"The customer management system. It should be straightforward."

Alex had looked at that API documentation the previous week. It was a REST service built in 2003 that returned XML responses with inconsistent field names and no error handling. Straightforward wasn't the word she'd use.

"On the count of three, everyone show your estimates," Sarah said. "One, two, three."

Alex held up an 8. Mack showed a 13. Jordan displayed a 5. Michael had chosen a 3.

Sarah looked confused. "We have quite a range here. Let's discuss. Michael, why did you estimate 3 points?"

"API integration is usually straightforward. Make the request, parse the response, handle errors."

"Mack, why 13?"

"Because I've seen this API. It's held together with duct tape and optimism. We'll spend more time debugging their responses than writing our integration code."

Jordan adjusted his estimate. "I was thinking 5 because we can probably work around the worst issues with some creative error handling."

Sarah made notes. "Alex, your thoughts on 8 points?"

"The API works, technically. But the documentation is incomplete, the error messages are cryptic, and we'll need to reverse-engineer half the functionality by trial and error."

"So we have estimates ranging from 3 to 13. Let's discuss until we reach consensus."

Alex watched Sarah facilitate the discussion with the earnestness of someone who believed that talking about problems would make them go away. Michael defended his optimistic estimate while Mack explained why every assumption about the API was probably wrong.

After fifteen minutes of debate, they settled on 8 points, which satisfied no one but fell within the acceptable range of dissatisfaction.

"Great! Let's move on to the CSV export feature."

Alex glanced at Mack, who was already shaking his head.

"This one should be simpler," Sarah continued. "We've already done the technical design work."

"Have we defined 'simple'?" Mack asked. "Because the last time I checked, this feature required a data classification engine, a consent management system, an approval workflow, rate limiting, encryption, and audit logging."

Sarah consulted her notes. "Those are implementation details. The user story is straightforward: export data to CSV."

"The implementation details are the actual work," Alex said.

"Right, but we can break those down into separate stories for future sprints."

Jordan leaned forward. "So we're estimating just the basic export functionality, without the compliance requirements?"

"Exactly. We'll tackle the compliance features in subsequent iterations."

Alex and Mack exchanged a look. They both knew that "subsequent iterations" was corporate speak for "never, but we'll pretend it's planned."

"If we're just building basic CSV export," Michael said, "that's probably a 3-point story."

"But we can't ship basic CSV export," Mack pointed out. "Legal won't approve it without the compliance features."

Sarah made a note. "We'll work with legal to define a minimum viable compliance framework."

"There's no such thing as minimum viable compliance," Alex said. "It's either compliant or it isn't."

"Let's estimate the basic functionality and address compliance in the next planning session."

They went through the planning poker ritual again. This time the estimates were closer—3, 5, 5, 8—but the discussion revealed that everyone was estimating different interpretations of the same requirement.

"I think we're converging on 5 points," Sarah announced.

"For functionality that we can't actually ship," Mack added.

"We'll iterate on the compliance requirements."

Jordan raised his hand diplomatically. "What if we approach this differently? Instead of estimating incomplete features, we could identify the smallest shippable increment and estimate that."

Sarah brightened. "That's a great agile principle. What would be the smallest shippable increment?"

"A CSV export that meets all legal requirements," Alex said.

"Which brings us back to the original 13-point estimate," Mack said.

Sarah looked at her notes, then at the index cards on the wall, then back at her notes. "Maybe we need to refine our user stories."

They spent the next hour breaking the CSV export feature into smaller pieces: "Data Classification," "User Consent Tracking," "Export Queue Management," "File Encryption," "Audit Logging." Each piece required its own planning poker session and generated its own disagreements about scope and complexity.

By the time they'd estimated all the sub-stories, they had 47 story points of work to implement a feature that users expected to be a single button click.

"This seems like a lot of points for CSV export," Michael observed.

"That's why we break it down," Sarah said. "Now we can see exactly what's involved."

"What we can see," Alex said, "is that we've turned a simple feature request into a quarter's worth of engineering work."

Jordan consulted the growing collection of index cards. "Are we planning to implement all of these sub-stories in the next sprint?"

"We'll prioritize based on business value and technical dependencies."

Mack laughed. "The business value is 'users can download their data as a spreadsheet.' Everything else is overhead created by our own processes."

Sarah moved to the next item on her agenda. "Let's look at the reporting dashboard. This is a high-priority request from Vincent."

Alex read the user story: "As a user, I want to see real-time analytics so that I can make data-driven decisions." She translated this as: "Vincent wants charts that look impressive in executive presentations."

"What kind of analytics?" Michael asked.

"Usage metrics, performance indicators, trend analysis. The usual dashboard components."

"Are we building this from scratch or using an existing framework?" Jordan asked.

"Vincent wants something custom that reflects our brand identity."

Mack held up his hands. "Custom dashboard framework is not a single user story. That's an entire product."

"We can start with basic charts and add features incrementally."

They went through the estimation process again, but this time the conversation devolved into a technical architecture discussion. Should they use a charting library or build custom visualizations? What about real-time updates? How would they handle data privacy for sensitive metrics?

After an hour of debate, they had seventeen sub-stories totaling 89 story points for what Sarah had originally described as a "basic reporting dashboard."

"I think we need to recalibrate our baseline," Jordan suggested diplomatically. "Our 1-point login story might not be representative of typical complexity."

Sarah looked at the wall of index cards, each representing weeks of engineering work. "Maybe we should schedule a follow-up session to refine our estimates."

"Or," Alex said, "we could acknowledge that software development is inherently complex and stop pretending we can predict timelines with Fibonacci numbers."

"The agile methodology is designed to handle complexity through iterative planning."

"The agile methodology is designed to make unpredictable work look manageable to people who don't understand the work," Mack said.

Sarah gathered her notes. "I think we've made good progress identifying the scope of our upcoming sprint. I'll work with Vincent to prioritize the stories based on business impact."

As people started packing up their laptops, Jordan approached Sarah. "This was a thorough planning session. Should we schedule regular retrospectives to refine our estimation process?"

Sarah's face lit up. "That's exactly the kind of continuous improvement thinking that makes agile work. Can you help coordinate the retrospective meetings?"

Jordan's smile faltered for just a moment. "I'd be happy to help."

Alex watched Jordan volunteer himself for more meetings while trying to look enthusiastic about it. His diplomatic instincts had backfired again, turning a simple suggestion into a new responsibility.

Mack was already at the door. "Same time next sprint?"

"Same time next sprint," Sarah confirmed. "And remember, we're committed to our velocity targets."

Alex looked at the wall of index cards representing months of work that Sarah expected to complete in two-week sprints. The agile transformation was going exactly as she'd predicted: more meetings, more planning, and the same amount of time to do the actual work.

She gathered her planning poker cards and left them on the table for the next team that would discover the gap between agile theory and engineering reality.
