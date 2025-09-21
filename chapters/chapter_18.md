# Chapter 18

The request looked reasonable in the ticketing system: “Export to CSV.” A button, a file, a download. The sort of thing that used to take an afternoon.

Legal was looped in by habit. Compliance joined because Legal was there. Security joined because Compliance was there. Brand joined because the button would be visible.

“We need to treat exported data like it can be forwarded to anyone,” Legal said.

“It can,” Alex said. “It’s a file.”

There was a pause in which the room became aware of itself.

—

Mack sketched an honest version on a whiteboard: gather rows, format commas, stream to disk, serve the file.

A compliance analyst uncapped a different marker and drew a fence around it. “Data classification. Consent tracking. Audit trail. Rate limiting. Encryption at rest and in transit. Expiration. Tamper-evident logs.”

“For a button,” Mack said.

“For a risk,” the analyst said.

Jordan translated. “What if we stage this in increments? Smallest shippable compliant piece.”

“Minimum viable compliance isn’t a thing,” Alex said.

“Then we write the whole thing,” Mack said. “Properly.”

—

They broke it into parts because that made it feel finite.

• Data Classification Engine: label each column as public, internal, confidential, restricted.

• Consent Registry: track whether a user had agreed to each restricted column’s export.

• Export Queue: process requests, avoid denial-of-service, pretend to be a platform.

• Encryption Pipeline: encrypt generated files with passphrases no one would remember.

• Audit Logger: record what was exported, by whom, when, with what keys, in a format Brand found readable.

• Retention & Purge: delete files on a timeline that satisfied three contradictory policies.

• Approvals: escalate exports over a threshold to a manager who would approve them at 11:59 PM.

—

Mack wrote the queue first. It was a polite queue with backoff. It stamped each request with an ID that could be traced through logs like a thread in fabric. He named the worker after a plant.

Alex took the classification engine. She resisted regexes that felt too clever and wrote a boring rule set from a dictionary the company already said it believed in. It turned out the company believed in three dictionaries.

Jordan mapped the approvals with words that would survive review: thresholds, exceptions, “fast path,” “slow path.” He left the owner field blank until someone volunteered.

Brand wanted the button placement to suggest responsibility. Alex put it in the corner where responsible buttons go.

—

Security’s policy required immutable logs. Legal’s draft added carve‑outs (“unless under counsel direction”). Compliance’s version mandated quarterly attestations and audit access. Each document made sense alone; together they didn’t.

"We’ll reconcile these" Jordan said.

"With who?" Alex asked.

Jordan shrugged.

—

The first end-to-end test produced a file that failed to open in the spreadsheet program that most people used.

“Unicode,” Mack said.

“Yes,” Alex said.

He fixed the encoding and broke the delimiter. The file opened as a single column that contained a convincing argument against computing.

The second test passed locally and failed in staging because staging had different data because staging had different everything.

The third test produced a zero-byte file and three perfect logs about the zero bytes.

“The system is compliant,” Jordan said.

—

They added an encryption step that produced files that could only be decrypted by people no one trusted with the passphrase. Security suggested splitting the passphrase into two shares. Compliance suggested three. Legal suggested sending both shares in separate emails “to reduce risk.”

Brand asked whether the download page could say something nicer than “Your file is encrypted.”

“We could say ‘Your file is safe,’” Jordan said.

“Are we sure?” Alex asked.

“We could say ‘Your file is ready,’” Jordan said.

Brand nodded. “That’s better.”

—

The approvals flow triggered at unexpected times: exports that should have been automatic asked for a signature; exports that should have been reviewed did not. The threshold logic was correct and also wrong, depending on whether you asked the policy doc or the business rule that had been explained verbally last quarter.

Jordan scheduled a meeting called Naming Things. It solved nothing and produced a glossary that disagreed with the policy doc.

—

Mack connected the audit logger to a place where logs were supposed to go. The place had been renamed the previous week and did not exist anymore. He created a new place and named it after the old place with a two appended at the end. He wrote a forwarder for the forwarder.

Alex wrote a health check that confirmed the system was alive and told no one whether it was doing the right thing. She added a metric that said export_attempted and sent it to a dashboard where numbers went to be admired.

Jordan drafted the communications for launch and created a FAQ that answered questions in a voice that sounded more confident than the system was.

—

Security ran a pen test and found a theoretical path to a file that did not exist. Legal read the report and added a line: “Address theoretical vulnerabilities in the next quarter’s cycle.” Compliance added: “Immediately.”

“Which is it?” Alex asked.

“Both,” Jordan said.

—

The pilot launched with a small group who actually needed the data. They clicked the button, waited in the queue, got their files, and opened them without reading the FAQ. One person pasted the content into a shared doc and asked whether anyone else could see the numbers.

"We’ll add a watermark," Brand said.

"CSV doesn’t have watermarks," Alex said.

"Then put the warning where they download it," Brand said. "Big, obvious."

"We can add a banner on the page and tag the filename ‘_CONFIDENTIAL’," Jordan said.

Brand nodded. "And a lock icon."

—

Two weeks in, the queue double-stacked with requests from a system no one admitted to owning. The exports were valid but empty because the consent registry contained entries for users who did not exist in the export source and therefore could not be matched and therefore returned nothing.

They built a temporary reconciler that merged two truths into one lie that satisfied both systems. It was documented under “operational notes” and assigned to no one.

—

Launch day arrived with a quiet banner and a quiet button. The queue stayed green, the logs went to the right place with the right labels, and the first bug report was about the phrase “Your file is ready.”

“What’s wrong with that?” Jordan asked.

“It sounds like it took too long,” Brand said.

Alex pressed the button, downloaded a file, and opened it on a machine not connected to anything. The commas were in the right places. The encoded characters decoded. The columns matched the columns. She closed the file and deleted it.

Mack looked at the dashboard and watched export_attempted increment without embarrassment. He added a panel that said export_completed and one that said export_denied and one that said export_confused for the cases that did not fit anywhere yet.

Jordan sent the launch note and scheduled a retro for a date the calendar rejected and then accepted again after it forgot it had rejected it.

—

That afternoon, a customer asked for JSON.

"We can do that," Vincent said from the doorway.

Jordan’s calendar populated: “JSON Export — Compliance Kickoff” and “JSON Export — Gate Review,” same attendees, same agenda.

