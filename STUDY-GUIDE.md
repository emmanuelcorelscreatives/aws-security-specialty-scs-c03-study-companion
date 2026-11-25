# AWS Security Specialty SCS-C03 — Study Guide

Use this guide alongside your practice tests to improve decisions, not memorize answers.

## Your practice course

- The course has six practice tests, each with 65 single-answer questions. Each test has a 170-minute time limit and an 80% practice benchmark. On a 65-question test, 52 correct answers reaches that benchmark.

- These settings help you structure practice. They are not the AWS exam scoring model, a prediction of an exam result, or a guarantee of readiness. The official exam may use question formats beyond the single-answer format used in this course.

- This is independent practice material, not an official AWS exam guide or a collection of actual or recalled exam questions.

## A useful study cycle

- Attempt one test without notes. Use the test timer, and flag uncertain answers so you can distinguish sound reasoning from guesses.

- After submitting, review all the explanations for missed or uncertain items. Name the deciding requirement: the principal, action, resource, policy layer, network path, timing, or evidence limit.

- Use the review worksheet to record the misconception in your own words. Do not copy entire questions or answer choices into shared notes.

- Read the relevant official AWS documentation using the reference index. Explain why an attractive alternative would solve a different problem.

- Revisit weak topics before attempting another test. Some security mechanisms recur across forms; remembered answer wording is not a substitute for applying the current scenario constraints.

## 1. Detection

- Separate collection from analysis and alerting. Establish which events are available before selecting an alarm or response workflow.

- CloudTrail management activity and object-level data activity are different collection categories. Enabling collection now does not reconstruct events that were never recorded.

- Treat log integrity and log completeness as separate questions. A digest-validation result concerns delivered evidence, not whether every required event category was selected.

- Trace a failed alert from ingestion through filters, metric generation, alarm evaluation, routing, destination permissions, and execution.

- Flow logs describe network metadata, not full application content. Check interface scope, traffic filters, collection status, and delivery timing before drawing conclusions.

- A central findings view supports triage. It does not remove the need to examine the producing service and confirm the affected account, Region, resource, and time window.

## 2. Incident response

- Prepare response owners, escalation routes, emergency access, and workload-specific procedures before an incident.

- Choose an exercise that matches the objective and safety boundary. A discussion-based rehearsal and a live tooling exercise establish different kinds of readiness.

- Distinguish stopping an exposed long-term key, stopping future role assumption, and containing previously issued sessions.

- Coordinate containment and evidence preservation. Verify the actual effect of a response action rather than relying only on a ticket update.

- Eradication addresses causes and persistence. Recovery requires trustworthy business operation, monitoring for recurrence, and an accountable operational handoff.

## 3. Infrastructure security

- Match edge controls to the threat. Request filtering, DDoS protection, user authentication, and origin access restriction solve different problems.

- Evaluate WAF changes against legitimate traffic before approved enforcement. Rate-based protection is not an exact business transaction ledger.

- Follow the complete network path. A firewall cannot inspect traffic that never traverses its endpoint; a stateful design also needs a coherent return path.

- Security groups and network ACLs have different state and rule semantics. Identify the control layer before deciding which direction or return ports need explicit rules.

- Use secure administrative access, workload roles, hardened metadata access, patching, and vulnerability assessment together. Verify service prerequisites instead of introducing an unnecessary public administration path.

## 4. Identity and access management

- Authentication establishes identity; authorization determines which request is permitted. Stronger authentication does not correct excessive authorization.

- Trace the actual principal and request context. Identity policies, resource policies, boundaries, session policies, and organization policies do not all behave identically.

- A permissions boundary limits an identity-policy grant; it does not independently supply that grant. Check explicit denies and the principal type before generalizing a policy result.

- For federation, check issuer, audience, subject, role trust, token validity, and the permissions of the resulting session.

- Separate successful workforce sign-in from account assignment and the permission set applied to the account. Review least privilege and update propagation as well as authentication.

## 5. Data protection

- Follow both the data path and the key authorization path. Access to a storage resource does not automatically grant use of its encryption key.

- Key rotation, secret rotation, ciphertext migration, and access revocation are different operations. Identify which one the requirement actually calls for.

- Preserve cryptographic dependencies for retained data. Immutable storage cannot recover destroyed key material.

- Object retention concerns particular versions. Distinguish fixed retention, legal holds, permitted extensions, and attempts to shorten a protected period.

- Check both sides of a transport connection. Front-end TLS does not by itself establish encryption on the backend connection.

- Data discovery identifies content and coverage limits. Sensitive content, exposure risk, and confirmed unauthorized transfer are different conclusions.

## 6. Security foundations and governance

- Use account structure, organizational controls, and delegated administration to establish clear management boundaries.

- Treat deployment scope, operation status, and per-resource results as separate evidence. A successful high-level operation does not always mean every target is in the intended state.

- Connect infrastructure policy checks to the release decision, and use live-resource evaluation for changes outside that deployment path.

- Configuration aggregation is a central view, not automatic rule deployment or remediation.

- Provider compliance documents, customer configuration evidence, and an auditor's compliance judgment serve different purposes. Check report scope, evidence relevance, and accountable review.

## Use the benchmark wisely

- Aim to explain the deciding constraint without looking at the choices. Review correct answers reached by guessing as carefully as incorrect answers.

- An 80% practice result is a useful course milestone, not an official certification decision. Combine consistent reasoning with study of the official objectives and hands-on experience where appropriate.

- AWS services evolve. Follow the current official documentation when it differs from older notes, and tell the instructor which course item may need review.

## Companion resources

- [Official reference index](REFERENCE-INDEX.md)
- [Review worksheet](REVIEW-WORKSHEET.csv)
- [Printable study guide](STUDY-GUIDE.html)
