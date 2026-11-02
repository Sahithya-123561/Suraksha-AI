Suraksha AI Dataset – Sources and Generation Method

1. Purpose

The Suraksha AI dataset contains examples used to develop, test, and evaluate the project's scam and digital safety detection modules.

It includes examples of suspicious messages, phishing attempts, online fraud, fake offers, and genuine messages.

The initial dataset is used for testing and calibration. It should not be treated as a complete training dataset.

2. Dataset Structure

Each dataset example should contain the following information:

id: Unique example ID.

category: Scam category or benign.

lang: Language used, such as English, Hindi, or Hinglish.

channel: Source type, such as SMS, WhatsApp, email, or social media.

text: Message or extracted text.

signals: Suspicious patterns identified by the detection engine.

label: 1 for scam and 0 for benign.

note: Short explanation of the example.

3. Scam Categories

The dataset can cover the following categories:

Digital arrest and impersonation scams.

Banking and KYC phishing.

UPI and payment fraud.

Fake job and recruitment offers.

Investment and cryptocurrency scams.

Courier and parcel scams.

Loan app and financial harassment.

Fake customer support and account recovery scams.

Suspicious links and phishing websites.

Genuine messages and normal conversations.

4. Data Sources

Dataset examples can be developed using patterns reported in:

Government cybercrime awareness materials.

Indian Cyber Crime Coordination Centre (I4C) advisories.

Reserve Bank of India (RBI) consumer awareness materials.

PIB Fact Check reports.

Public cybersecurity research.

Publicly available phishing and scam datasets.

Open-source scam detection projects, following their licenses.

Examples should be paraphrased or created as synthetic messages. Do not include real victims' names, phone numbers, bank details, or other personal information.

5. Dataset Generation Method

The dataset can be developed in stages:

Stage 1: Initial examples

Prepare a small set of manually written scam and genuine examples.

Assign categories and labels.

Check whether the examples match the intended detection rules.

Stage 2: Dataset expansion

Add more examples using carefully written templates.

Include different languages and writing styles.

Cover SMS, WhatsApp, email, and social media messages.

Include both scam and genuine examples.

Stage 3: Testing dataset

Keep separate examples for testing.

Avoid using the same examples in both development and final evaluation.

Check detection results against the expected labels.

6. Dataset Quality Rules

Include both scam and benign examples.

Avoid duplicate messages.

Use correct labels and categories.

Include English, Hindi, and Hinglish examples where supported.

Protect personal information.

Test new examples before adding them to the main dataset.

Monitor false-danger predictions on genuine messages.
