# Chapter 12

The subject line said it was routine. The calendar invites said otherwise.

Alex skimmed the message. ByteSauce was conducting a "standardized security posture review." All engineering teams. This week. A shared spreadsheet tracked time slots like a hospital intake board.

Jordan messaged: "I'll sit in."

Mack: "Do we have a posture?"

---

The auditor introduced himself as Greg and did not shake hands. He carried a tablet, a checklist, and the energy of someone who preferred boxes checked to conversations had.

"I'll start with access controls," he said, already opening tabs. "Then code review protections, password policies, credential storage, deployment gates. Standard order."

Jordan smiled like he was glad standards existed. "Happy to walk you through our process."

Greg was already in the repository settings. "Main is open to direct push."

Alex glanced at the screen. "It's… historically open."

"How long has it been open?"

"Since we created it."

Greg tapped something on his tablet. The sound felt like a timestamp.

"Branch protection should be enabled. Required reviews should be enforced. Dismiss stale approvals. Status checks required."

"We can enable those," Jordan said. "Today."

Greg didn't look up. "Today would have been better two years ago. Credentials?"

Alex opened the secrets page for their deployment system. She hesitated for half a breath before scrolling.

Greg read. "Plain text in a shared notes tool. Development database password is 'password'."

Mack scratched his neck. "It's development."

"It's a password," Greg said. He didn't raise his voice. "Shared notes tool has no audit log."

Jordan kept his voice even. "We can migrate to the password manager. The corporate one."

"It timed out for three months," Alex said. "That's why we…"

Greg made another note. "The tool being broken is not an exception policy."

---

In the conference room, the TV reflected Greg's checklists at a slight delay, as if the system itself needed time to process the implications.

"Code review," Greg said. "I see references to an Innovation Score rubric in your PR template."

Mack glanced at Jordan. "Historical artifact."

Greg clicked into a merged pull request. The diff contained three lines of working code and twenty lines of commentary about "paradigm-shifting statistical engines."

"What is this?" Greg asked, neutral.

Jordan considered the safest version of the truth. "A leadership initiative incentivized… visible creativity in reviews. It created noise. We can remove it."

Greg scrolled. "It created noise. Yes. Who approved this one?"

Alex swallowed. The approving user icon was theirs.

"We'll remove it," she said. "Today."

Greg nodded. "Remove the rubric. Enable protections. Migrate credentials. Document the deployment gates. I'll need evidence."

He closed the laptop with care, as if to avoid smudging anything further.

---

After he left, no one said anything for a minute. It wasn't a dramatic silence. Just the kind that happens when the facts have finished arranging themselves.

Jordan exhaled first. "I'll file the requests for branch protection and status checks."

"I'll move the credentials," Alex said. "And rotate the ones we hard-coded in the runbook we pretend is a wiki."

Mack opened his terminal. "I'll strip the Innovation Score blocks from recent merges and update the PR template."

Jordan nodded. "And I'll draft a summary for Sarah. Minimal adjectives."

Alex opened the repo settings. The toggles were exactly where Greg said they'd be. She enabled one, then another. Each switch felt like a belated apology written in UI.

A notification popped up in Slack: "Security posture review: please upload remediation evidence here." There was a link to a folder with their team name and a placeholder file called evidence.txt.

Alex created a real one and started dropping screenshots into it. The folder name looked like something that would be referenced later by someone who didn’t know any of their names.

She set her laptop to upload and watched the progress bar move across the screen in a straight, unambiguous line.

---

Sarah appeared in the doorway like a question mark.

"How bad?" she asked.

Jordan angled the monitor away from her on reflex. "Manageable."

Sarah looked tired in a way that lights couldn’t correct. "I'll need two sentences for leadership."

Jordan nodded. "We identified gaps in access controls and credential storage; remediations are in progress with evidence attached. Timelines: by end of week."

"That'll work," Sarah said. She lingered half a beat. "If there are landmines I should step on before someone else does, tell me."

"We'll surface them," Jordan said. He meant "we’ll defuse them and leave the shards."

Sarah left as quietly as she'd arrived.

---

Alex wrote a small script and didn’t tell anyone. It looked for strings that smelled like secrets—base64 blobs, aws_ prefixes, anything ending in _KEY or _TOKEN—in every repo she had access to. It pinged empty directories like a sonar. The output wasn’t pretty, but it was honest.

She found three credentials in old Jenkins job definitions, two in a Terraform variable file from a migration that never happened, and one in a shell script that had survived four reorganizations because no one knew what it did but also no one was brave enough to delete it.

She rotated what she could and documented what she couldn’t.

For the ones she couldn't rotate without downtime, she created temporary compensating controls, which is what you called it when you built fences around bad decisions.

---

Mack pulled up the PR template and removed the Innovation Score block. He didn’t make a speech about it. He just deleted the lines and added a note that said "Keep changesets small. Add tests."

Then he went hunting.

ripgrep turned up every "INNOVATION SCORE:" in the codebase. Most were jokes. Some had been cargo-culted into new files by people who thought they were following a rule.

He scrubbed them quietly and rebased the noise away where he could. He left the actual work visible.

He also wrote a one-off script to rotate a handful of internal tokens and pushed it to a private repo named after a plant, because that was the closest he came to plausible deniability.

---

Jordan opened Confluence and created a page titled "Security Hygiene (Working)." He wrote in short lines and bullet points and avoided any sentence that sounded like a policy. He linked to the evidence folder, the branch protection settings, and a checklist with boxes that could be checked by anyone with a mouse.

He DM'd Greg. "We'll attach evidence as we remediate. Please reply 'received' for each upload so we have an audit trail."

Greg replied with a thumbs-up emoji and a timestamp. It was the most human thing he had done all day.

Jordan added a line to the page: "Acknowledgements captured in thread." It looked official without sounding proud of itself.

---

By late afternoon, they had a rhythm. Alex found secrets; Mack rotated what he could reach; Jordan turned their work into receipts.

Someone from another team asked in a public channel whether the "innovation rubric" would be returning. No one answered. The message scrolled out of view beneath a cascade of status updates and meeting links.

Vincent posted a company-wide note reminding everyone to "keep shipping against Q3 OKRs" and to "use this audit as a chance to demonstrate our operational excellence." He wrote "operational excellence" three times in two paragraphs. It read like he was trying to convince himself.

Sarah reacted with a checkmark and nothing else.

---

Greg returned for a short follow-up, which consisted mostly of him opening their evidence folder and asking for screenshots with the browser chrome visible.

"We prefer showing full context," he said. "It reduces disputes later."

"Disputes?" Mack asked.

Greg didn’t answer. He was already counting the toggles in a screenshot with his finger.

He stopped at the PR template diff. "Good. Remove the rubric from the template and from cultural practice."

"From cultural practice," Jordan repeated, as if it were a setting.

Greg closed his tablet. "I'll compile a preliminary report. You'll get the official one next week. Continue uploading evidence."

He left a small stack of printed guidance on the corner of the table. No one touched it.

---

The plain-text password in the shared notes tool became a Slack thread no one reacted to in public. Alex moved it to the password manager, updated the environment variables, and pushed a tiny change that did nothing but forced a new deployment so the secrets would refresh.

The deploy took three minutes. The logs rolled by like a polite parade. Nothing broke. Alex was almost disappointed.

She added a line to the runbook that said, "This exists," with a link.

---

At five-thirty, the floor got loud with coats and laughter from other departments. Engineering stayed seated.

Jordan rewrote his summary for Sarah four times until it didn’t sound like an apology.

- Access controls: enforced branch protection, required reviews, status checks. Evidence attached.
- Credential storage: migrated to password manager; rotations in progress; compensating controls documented.
- Code review template: removed non-functional rubric; added test and changeset guidance.

He sent it and nudged the lid down without closing it.

---

Alex's script finished its last pass and printed a final list of suspicious matches. She sorted them by confidence and assigned the lowest to "monitor."

She considered turning the script into a pre-commit hook and then didn't. They needed fewer rules, not new ones written by the same people who didn't follow the old ones.

She archived the script in a folder named tools and wrote a readme that said, "Use if needed."

---

Mack created a tiny internal page titled "Things That Are Now True" and listed five bullets that no one would argue with.

- Main is protected.
- Reviews are required.
- Tests are not optional.
- Secrets live in the tool with the lock icon.
- The template is smaller.

He turned off notifications for the page.

---

Greg's shared folder pinged again. "Please upload evidence of password rotations." There was a specific format requested for filenames: teamname_artifact_date.png.

Alex renamed her screenshots. It was easier than asking whether the underscore mattered.

She watched the progress spinner until it became a checkmark.

---

On the way out, they passed Sarah talking to Legal in the hallway. The conversation used words like "exposure" and "mitigation" in voices calibrated not to carry.

Sarah caught Jordan's eye and gave a small nod that meant "I saw your summary" and also "thank you for making it look like this."

Jordan nodded back. He didn’t say anything because the right word would have sounded like a promise.

---

It was dark outside. The motion sensor lights in the conference room clicked off and then on again as Alex went back for her water bottle. The TV still reflected the last checklist they had closed.

She unplugged the HDMI, and the reflection disappeared.

On her desk, the evidence folder was still open. She added one more screenshot—the branch protection page with all the toggles green—and dragged it into place.

The upload bar moved from left to right, steady and unremarkable, the way good decisions look when they happen too late to be dramatic.

By morning, the evidence folder had a new observer no one invited.
