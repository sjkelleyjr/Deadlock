# Chapter 12: The Security Audit

The email arrived at 8:47 AM on a Tuesday morning, which was suspicious timing. Corporate emails never arrived before 9:00 AM unless something was wrong.

"URGENT: ByteSauce-Wide Security Review - All Engineering Teams Must Comply"

Alex read it twice, then forwarded it to the team Slack with a single word: "Shit."

Jordan responded first: "What's the actual scope?"

Mack: "Define 'security review'"

Sarah chimed in: "Corporate is concerned about recent 'productivity improvements' and wants to ensure we're following security best practices."

Alex stared at the screen. "They're investigating us."

---

The security auditor arrived at 10:00 AM sharp. His name was Greg, and he wore a polo shirt with a company logo that looked like it had been designed by someone who'd never seen a computer. He carried a clipboard and spoke with the confidence of someone who'd read exactly one cybersecurity article.

"Good morning, team. I'm here to conduct a comprehensive security review of your development practices."

Jordan smiled warmly. "Welcome, Greg. We're happy to help with any security concerns."

"Excellent. Let's start with your password policies."

Alex felt her stomach drop. She'd been storing test credentials in a plain text file for the last three months because the company's password manager was so broken it took fifteen minutes to retrieve a single password.

Greg opened his laptop and began typing. "First, I need to see your current password storage practices."

Mack leaned back in his chair. "Define 'password storage practices.'"

"Well, how do you store passwords for development environments, databases, API keys, that sort of thing?"

Jordan glanced at Alex, then at Mack. "We follow company policy, of course."

"Of course. And what is company policy?"

Alex cleared her throat. "We use the corporate password manager."

Greg nodded approvingly. "Good. And how often do you rotate passwords?"

"According to policy," Jordan said smoothly.

"Which is?"

"Quarterly," Alex lied.

Greg made a note. "Excellent. Now, let's look at your code repository security."

Mack's eyes narrowed. "What exactly are you checking?"

"Access controls, branch protection, code review processes, that sort of thing."

Jordan smiled. "We have a very robust code review process. In fact, we recently implemented an Innovation Score system that ensures all code meets our quality standards."

Greg's face lit up. "Innovation Score? That sounds cutting-edge. Tell me more."

Alex felt the trap closing. The Innovation Score system they'd gamed with fake comments was about to be exposed as a security risk.

"Each code review gets scored on innovation and creativity," Jordan explained. "It helps ensure we're building truly disruptive solutions."

"Fascinating. And how do you prevent malicious code from being merged?"

Mack leaned forward. "We have automated tests."

"Which run when?"

"Before merge," Alex said quickly.

Greg typed something on his laptop. "I see. And what about your production deployment process?"

Jordan's diplomatic smile never wavered. "We follow industry best practices."

"Such as?"

"Automated testing, code review, approval workflows."

Greg nodded. "Good. Now, let me check your actual repository settings."

He opened his browser and navigated to their Git repository. Alex watched as he clicked through the settings, her heart rate increasing with each click.

"Interesting," Greg said. "I notice that your main branch doesn't have branch protection enabled."

Jordan's smile faltered slightly. "We're in the process of implementing that."

"Process of implementing? How long has this repository been active?"

"About two years," Alex admitted.

Greg's eyebrows rose. "Two years without branch protection? That's a significant security risk."

Mack crossed his arms. "How significant are we talking?"

"Anyone with write access could push directly to main, potentially deploying malicious code or breaking the application."

Jordan nodded thoughtfully. "You're absolutely right. We should prioritize this."

"Priority one," Greg said, making another note. "Now, let me check your recent commits."

Alex felt her palms start to sweat. The Innovation Score comments were going to be visible in the commit history.

Greg scrolled through recent pull requests. "I see some interesting commit messages. 'REVOLUTIONARY AI-POWERED STATISTICAL ANALYSIS ENGINE' - that's quite descriptive."

Mack's jaw clenched. "We believe in clear, descriptive commit messages."

"Very clear. And these comments in the code - 'INNOVATION SCORE: 8.9/10' - what's that about?"

Jordan cleared his throat. "That's part of our quality assurance process."

"Quality assurance? These comments don't seem to relate to the actual code functionality."

Alex felt the walls closing in. "They're documentation standards."

Greg frowned. "Documentation standards that include innovation scores? That seems unusual."

Mack leaned back in his chair. "What makes it unusual?"

"Unusual as in, I've never seen anything like this in a professional codebase. It looks like someone is gaming a system."

Jordan's diplomatic facade cracked slightly. "Gaming? That's a strong word."

"Is it? Because these comments appear to be artificially inflating some kind of scoring system rather than providing actual code documentation."

Alex felt the trap snap shut. "We can explain the Innovation Score system."

"Please do."

Jordan took a deep breath. "It's a corporate initiative to encourage innovative thinking in our code."

"By adding fake comments about AI and machine learning to simple arithmetic functions?"

Mack's chair creaked as he shifted. "The comments are aspirational."

"Aspirational? For a function that calculates the average of an array?"

Alex felt her face flush. "The system was designed to encourage creative thinking."

"Creative thinking about how to deceive management, perhaps?"

Jordan's smile was now completely gone. "I think there's been a misunderstanding."

Greg closed his laptop. "I think the misunderstanding is on your end. You've been systematically gaming a corporate system, and in the process, you've created a codebase that's both insecure and unprofessional."

Mack stood up. "Unprofessional? We've been doing our jobs while dealing with impossible requirements and meaningless metrics."

"By lying to management?"

"By surviving," Alex said quietly.

Greg looked at each of them in turn. "I'll be filing a report with corporate. This goes beyond security issues - this is a fundamental breakdown in professional standards."

Jordan tried one more diplomatic approach. "Greg, I think we can work together to address these concerns."

"Address them? You've been actively subverting company policies for months. This isn't something you can 'address' with a meeting."

Alex felt the weight of their previous victories crashing down. The Innovation Score gaming, the budget meeting research project, the team building subversion - it was all coming back to haunt them.

"Greg," she said, "we can fix the security issues immediately. Branch protection, proper password management, real code reviews."

"Fix them? You should have had them from the beginning. The fact that you're only addressing basic security practices now, after being caught gaming the system, suggests a fundamental lack of professional judgment."

Mack's hands were clenched into fists. "Professional judgment? We've been dealing with a system that rewards buzzwords over actual work."

"Then you should have raised those concerns through proper channels."

Jordan laughed bitterly. "Proper channels? We've been trying to work within the system for months."

"By lying to it?"

Alex felt the conversation spiraling out of control. "We can implement proper security practices starting today."

"Today? You should have had them implemented two years ago. This isn't about implementing security practices - this is about a team that's been systematically deceiving management."

Greg stood up and gathered his things. "I'll be submitting my report by end of day. I recommend you start preparing your responses to corporate."

After Greg left, the team sat in stunned silence.

"Well," Mack said finally, "that could have gone better."

Jordan rubbed his temples. "We're going to need to do some damage control."

Alex stared at her screen. "Damage control? We just got caught gaming the Innovation Score system that we've been using for months."

"Not just gaming it," Mack added. "We made it look like we were building revolutionary AI systems when we were just writing basic functions."

Jordan nodded slowly. "And now corporate knows we've been lying to them."

Alex felt the consequences of their previous victories settling in. "We've been getting away with too much. It was bound to catch up with us."

Mack stood up and started pacing. "So what do we do now?"

"First," Jordan said, "we implement real security practices. Branch protection, proper password management, actual code reviews."

"Second," Alex added, "we prepare for the corporate investigation."

"Third," Mack said, "we figure out how to survive this without losing our jobs."

Jordan looked at his phone. "I should probably call Sarah. She's going to need to know about this."

Alex opened her terminal and started typing. "I'll set up branch protection on the main repository."

Mack sat back down. "I'll start removing the fake Innovation Score comments from our recent commits."

Jordan nodded. "And I'll draft a response to corporate explaining our security improvements."

As they worked, Alex felt the weight of the situation settling in. Their previous victories had consequences, and the company's dysfunction was becoming more dangerous. The game was getting harder to play.

She typed the command to enable branch protection and wondered how much longer the game would continue.
