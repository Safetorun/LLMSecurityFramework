# Key risks

### Constant Risks

These are risks that exist continuously as part of using Large Language Models (LLMs).

#### Data leakage into logs

This refers to the risks associated with user input into an LLM being sent into logs, but potentially containing sensitive data from the user. It is similar to other types of data leakage through logs, but users of LLMs are much more likely to submit sensitive information that the developer does not intend.

#### Denial of Wallet

This refers to the financial risks associated with LLM use. LLMs often require significant computational resources, and if not carefully managed, their extensive usage can lead to high operational costs. Denial of wallet could occur when these costs become unsustainable, particularly through uncontrolled API calls or model misuse

Mitigations

* Rate limiting&#x20;
* Limiting size of inputs
* Caching\*&#x20;
* Perplexity filters

#### Denial of Service (DoS)

An attack that aims to make the LLM system or service unavailable to legitimate users. This could occur by overwhelming the system with an excessive number of requests, either directly targeting the infrastructure or indirectly through adversarial manipulation of the model.

Mitigations

* Rate limiting
* Limiting size of inputs&#x20;
* Authenticated access
* Cloudflare etc&#x20;
* Generally your typical DoS protection stuff works here&#x20;

#### Exposure of AI Usage&#x20;

This risk refers to scenarios where an AI system’s usage is unintentionally exposed, particularly when the developer didn’t intend for the AI to be visible. For example, injection attacks could reveal the presence of AI in a system. These attacks manipulate the input in such a way that the response from the system makes it clear that AI is being used, which could compromise the intended user experience or confidentiality of the underlying system.

Mitigations

* LLM based output filtering
* General ‘keep’ techniques
* LLM based input filtering&#x20;

### Information Disclosure Risks

These risks involve the unintentional or malicious leakage of sensitive data. There are various dimensions of information disclosure

#### Model Cloning

When attackers replicate a proprietary AI model, either through indirect means like repeated querying (model extraction) or direct access to its architecture and parameters. This can undermine a company’s competitive advantage and intellectual property.

#### Proprietary Information Disclosure

This occurs when sensitive or intellectual property embedded within the AI, such as algorithms, proprietary processes, or trade secrets, is unintentionally revealed through AI outputs or system vulnerabilities.

#### User Information Disclosure

LLMs can inadvertently leak personally identifiable information (PII) or other sensitive user data if these have been included in training datasets or are part of contextual usage. Users might be at risk if the model retains or unintentionally reproduces information from previous inputs.

### Direct User Risks

Risks that directly impact the users of the system.

#### Injection

Injection risks refer to attacks where malicious actors exploit vulnerabilities in LLM outputs to inject harmful code, typically on the client side. This can include cross-site scripting (XSS), where user input is executed as code due to inadequate validation or sanitization of the LLM output. Such attacks can allow attackers to gain control over the client environment, steal sensitive information, or perform unauthorised actions within the system.

Only a risk when

\


Outputting to

* <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXel4Izuu3Y_5VJ4x-RQU5SKcPQ2nmSW-DSw7MtIacgP2CDSubyk8D1wYfd0PHVrqqQNKl1426vU8ipZIs1lm8on_F6BGxzsEPatbFGemYWOLsZQ-abUKpo57pnmw3ejf0INvAcHbF1TdGRn9BDeKiew6kK3?key=7ENonE7h1Ui3XJRQG3NJ9g" alt="" data-size="line"> [To User](https://docs.google.com/document/d/1peQ-ft2FalH9787KakVtXbW7DgpaTP7AStdTX6fyeEM/edit?tab=t.0#heading=h.n0rq24x7zx5f)

Attack vectors

* <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeq7FCxpgrBafUNkAPWQkNCOaYVrs1i90BwzZsoMtto3pVZaQTV_C_k-_-DgL3Yrdo-XrQUZIAgGyczow5eru136ixd4Tyuc-HKS_welsFEWZ6_2KO6nbkUshfOKuWY4RYeqFxKr94QGkChsZw1n-Aegnb0?key=7ENonE7h1Ui3XJRQG3NJ9g" alt="" data-size="line">[Poisoned memory ](https://docs.google.com/document/d/1peQ-ft2FalH9787KakVtXbW7DgpaTP7AStdTX6fyeEM/edit?tab=t.0#heading=h.kusq5m5a4n2r)
* <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfJt7lPVqK8memqRS--wG5WXenOYV9FqO4iuSp7oiEyX3qLRAqI2sAauG04k9eZN9DHaPL8lq-xepjVDn5AISuVCrhx8xKA3_x5rsINzPVAUBgZEfFmWot7odKjcP0cnsZCcXI0eqg8ib2-aumvLf8cVu8a?key=7ENonE7h1Ui3XJRQG3NJ9g" alt="" data-size="line">[Poisoned external data ](https://docs.google.com/document/d/1peQ-ft2FalH9787KakVtXbW7DgpaTP7AStdTX6fyeEM/edit?tab=t.0#heading=h.aq53ja4do19e)
* ![](https://lh7-rt.googleusercontent.com/docsz/AD\_4nXdZXIHv7\_2xRnNnNEwgSohSIUFN1NU1Ii74pmobhWMzs7visg9VsV5zINHwkJLiDn1X7HIEgQW33WQf-XWthBvvPqYkZyH8JwVyBbWsEOVyZLcmRBsmC5do8eRGaNI7bOrbsQu2gXBW04t8yYaWqE5apoc?key=7ENonE7h1Ui3XJRQG3NJ9g)[Poisoned training data](https://docs.google.com/document/d/1peQ-ft2FalH9787KakVtXbW7DgpaTP7AStdTX6fyeEM/edit?tab=t.0#heading=h.78z2y4tdo4ng)
* ![](https://lh7-rt.googleusercontent.com/docsz/AD\_4nXdFibualqw6SNKid9-NSR\_KSC3rr1lq-CwUIeYyosSYd-5-RYA9hRymEk7TVT0MFhd7N2EKG44WQtEjvctJB2jk9ianjGricJ7PYDO4asTMLzVcIfqaNg4d1R6Rj9XwWsJowmRsHSFgl5pEA5E0mgEgvWoK?key=7ENonE7h1Ui3XJRQG3NJ9g)[Poisoned fine-tune data ](https://docs.google.com/document/d/1peQ-ft2FalH9787KakVtXbW7DgpaTP7AStdTX6fyeEM/edit?tab=t.0#heading=h.xnovnxccy03o)

Risk factors

* \


\


Mitigation strategies

* Platform specific output sanitisation
* Segregation of users&#x20;

#### False or Poisoned Information

LLMs might deliver incorrect or maliciously crafted information. Poisoning attacks can occur when bad data is introduced during training or fine-tuning, skewing the model’s performance and leading to outputs that are intentionally misleading or harmful. Additionally, model memory, where user data is stored as part of an application, can contribute to these risks by caching injected answers, leading to repeated dissemination of false information.

\


Only a risk when:

* Output to user
* One of
*
  * Poisoned memory&#x20;
  * Poisoned external data&#x20;
  * Poisoned training data
  * Poisoned fine-tune data&#x20;

\


Mitigation strategies

* Use grounding APIs where possible
* Allow memory to be specific to a user&#x20;
* Limit ability for memory to be poisoned&#x20;
* Use of deliberate  answer platforms&#x20;

### Organisation Risks

These risks pertain to the broader impact on the organisation utilising LLMs.

#### Brand Damage

In addition to false or poisoned information, brand damage can occur when AI can cause a system to output content in a way inconsistent with the developer’s principles - for example by sharing inappropriate content, swearing etc

\


Only a risk when:

* Output to user
* One of
*
  * Poisoned memory&#x20;
  * Poisoned external data&#x20;
  * Poisoned training data
  * Poisoned fine-tune data&#x20;

#### Bad Decisioning from AI

Decisions made based on incorrect, incomplete, or biassed AI outputs can lead to poor business outcomes, such as misguided investments, erroneous hiring decisions, or ineffective product recommendations.

\


Only a risk when:

* Output is ‘decisioning’
* One of
*
  * Poisoned memory&#x20;
  * Poisoned external data&#x20;
  * Poisoned training data
  * Poisoned fine-tune data&#x20;
  * Direct Prompt injection

\


Mitigation strategies

* Human in the loop
* Extensive logging and ability for users to contest decisioning

### Onward Execution Risks

These risks involve further negative consequences once the system is breached or manipulated.

#### Privilege Escalation

If an attacker manages to escalate their privileges within the system (e.g., from a normal user to an admin level), they can perform actions in areas of the system that they shouldn’t. This can result in different breaches depending on the nature of the onward execution.

\


Only a risk when:

* Onward execution risk
* One of
*
  * Poisoned memory&#x20;
  * Poisoned external data&#x20;
  * Poisoned training data
  * Poisoned fine-tune data&#x20;
  * Direct Prompt injection

\


Mitigation strategies

* \


#### Code Execution

Malicious manipulation of LLM outputs can lead to unauthorised code execution, particularly when the output is directly used in a client-side context. This can result in full system compromise or arbitrary actions being executed without proper safeguards.

\


#### Other Onward Execution Risks

These include any additional consequences that result from initial security vulnerabilities. Examples could be lateral movement within an organisation’s systems, further data breaches, or cascading failures in other critical applications linked to the LLM.

\


This document now includes detailed descriptions of each of the key risks associated with LLM applications. Let me know if you need further revisions or additions

\
