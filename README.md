ANONYMOUS FEEDBACK APP


People want honest feedback but fear social awkwardness
More honest feedback = faster professional growth
Companies want feedback culture but struggle to create safe spaces
Sits between casual Slack convos and formal performance reviews

Core Concept
Employees give each other constructive feedback without revealing who said what, helping people understand their blind spots and grow professionally without the awkwardness of face-to-face criticism.
Verification System
Company Email Verification

Users sign up with their work email (e.g., sarah@company.com)
Send verification link to confirm employment
After verification, the email is hashed/encrypted and the original is deleted
User creates a separate anonymous profile with no identifiable info

Optional: LinkedIn Integration

Cross-verify employment status
Import job title/department (stored separately from identity)

How Feedback Works
Requesting Feedback

You generate a unique shareable link (like "give feedback to Employee #47382")
Share it with colleagues via Slack, email, or in-person
Recipients don't need accounts to submit feedback initially, but need one to receive feedback themselves

Giving Feedback

Anonymous by default - the system never stores who said what
Structured prompts like:

"What should this person keep doing?"
"What's one area for improvement?"
"How effectively do they communicate?"


Mix of ratings and written feedback
Character limits to encourage thoughtful responses

Reading Feedback

Aggregate view showing patterns across multiple responses
Individual comments (all anonymous)
Sentiment analysis highlighting themes

Anonymity Architecture
Technical Separation

Identity database (who works where) is completely separate from feedback database
Feedback is submitted through an anonymizing layer
Not even admins can connect feedback to individuals
Use one-way hashing for any linking that's needed

Preventing De-anonymization

Minimum threshold (e.g., need 3+ responses before revealing any feedback)
Strip metadata from submissions
Rate limiting per anonymous session
Fuzzy timestamps ("2 days ago" not "2:47pm on Tuesday")

Trust & Safety
Preventing Abuse

NLP to flag potentially harmful content before posting
Report mechanism for inappropriate feedback
Verified humans only (no bot spam)
Option to require mutual feedback (you must give to receive)



Reputation system (good feedback-givers get badges)
Require minimum character counts
Block generic/lazy responses
