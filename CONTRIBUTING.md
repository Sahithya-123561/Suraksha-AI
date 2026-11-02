Contributing to Suraksha AI 🛡️

Thank you for helping us make digital platforms safer. Suraksha AI aims to help people identify online scams, suspicious messages, phishing links, and potentially manipulated media.

Please follow these guidelines when making changes to the project.

1. The Main Rule: Test Every Change

Every code change must be tested before it is added to the main project.

Run the available project tests:

node engine/gate.mjs

This command should be used if the gate script is present in the repository. It checks the engine, runs available tests, and verifies supported evaluation rules.

Before submitting changes:

Run the available test scripts.

Check that existing features still work.

Fix errors introduced by your changes.

Do not reduce detection quality or increase false warnings without investigation.

2. Follow the Project Structure

Keep frontend, backend, and detection modules organized.

Follow the existing project structure.

Avoid unnecessary changes to working detection logic.

Do not modify generated engine files directly if they are created by an extraction script.

Update the original source file and regenerate derived files using the project's documented process.

3. Adding New Scam Detection Features

When adding new scam detection patterns:

Add rules for suspicious messages and online fraud.

Include examples of genuine messages to prevent false warnings.

Support Indian scam categories such as UPI fraud, fake job offers, banking scams, and digital arrest scams.

Add clear explanations for every important detection result.

Support English, Hindi, and Hinglish where implemented.

Test both suspicious and genuine examples.

4. Adding Image, Audio, and Video Features

When contributing to media analysis:

Support only the file formats implemented by the application.

Validate uploaded files before processing.

Handle corrupted or unsupported files safely.

Do not claim that an image, audio file, or video is fake without sufficient evidence.

Clearly explain when a detection method is unavailable or inconclusive.

5. URL and QR Code Security

When improving URL and QR analysis:

Check suspicious URL patterns.

Identify potentially misleading or look-alike domains.

Analyze URLs extracted from QR codes.

Test with both safe and suspicious links.

Never automatically open an untrusted link.

6. Principles of Suraksha AI

Every contribution should follow these principles:

User safety: Help users recognize possible online threats.

Accuracy: Avoid unnecessary false warnings.

Transparency: Explain why content is marked suspicious.

Privacy: Do not store user-submitted messages or media unless an explicitly documented feature requires it and users are informed.

Simple language: Keep explanations easy to understand.

Responsible detection: Results are risk assessments, not guaranteed proof that content is real or fake.

Emergency support: Keep the Indian cybercrime helpline 1930 visible in relevant safety guidance.

7. Before Submitting Changes

Check the following:

Code follows the existing project structure.

New features have been tested.

Existing features still work.

Invalid inputs are handled correctly.

No unnecessary user data is stored.

Detection explanations are understandable.

Documentation is updated.

Available project tests pass.
