# Attack vectors

### <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXe4Gh6xS_lhbSqGs_ihT3ujxoVrPHEnUsX7XN1SwbNrLGz2KG7IMOrLDfqvgS40UTs3Se88YqCjSdg11bTkwJUl1omoxGzrqrgQ20CqJJfyKxvzoJ_6Ukxx4j1noJ2JmMmgvwqIvUX0AClEvOkec86Dqp6J?key=7ENonE7h1Ui3XJRQG3NJ9g" alt="" data-size="line"> Attack vectors&#x20;

Attack vectors are the mechanisms by which input can be tainted in such a way as to impact the correct functioning of an AI Application

#### <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXf3_fSTu9zTa1A9-Tb6AfzibiDZ065o9CGVdzqb6m74ODm_fUqGL-qySmFV-mx68J9gvpguqSnH72Lr9NDAiHoxmcpWMk7xncFWdWp7slgi3oQP8nsGReTa3he6L5g6oyr_QpOxtHgPbvnZTe2FUErTDsA2?key=7ENonE7h1Ui3XJRQG3NJ9g" alt="" data-size="line">Direct Prompt Injection

* What it is: An attacker directly inserts malicious instructions or manipulative commands into the prompt given to the LLM. This bypasses any filtering applied to external data or training data, going straight to the LLM's interpretation engine.
* Example: An attacker might craft a prompt that tricks the LLM into revealing sensitive information from its memory, changing its personality settings, or generating harmful content.
* What it means: This is a high-risk attack as it directly exploits the way the LLM processes information. It can lead to data leakage, generation of inappropriate content, or manipulation of the LLM's behaviour.

#### <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfJt7lPVqK8memqRS--wG5WXenOYV9FqO4iuSp7oiEyX3qLRAqI2sAauG04k9eZN9DHaPL8lq-xepjVDn5AISuVCrhx8xKA3_x5rsINzPVAUBgZEfFmWot7odKjcP0cnsZCcXI0eqg8ib2-aumvLf8cVu8a?key=7ENonE7h1Ui3XJRQG3NJ9g" alt="" data-size="line"> Poisoned External Data

* What it is: An attacker injects malicious or biassed information into the external data sources that the LLM uses for retrieval augmented generation (RAG).
* Example: An attacker might tamper with a website or document that the LLM uses for RAG, inserting false information, propaganda, or links to malicious websites.
* What it means: This can cause the LLM to generate inaccurate, biassed, or harmful outputs, potentially spreading misinformation or manipulating users.

#### <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdZXIHv7_2xRnNnNEwgSohSIUFN1NU1Ii74pmobhWMzs7visg9VsV5zINHwkJLiDn1X7HIEgQW33WQf-XWthBvvPqYkZyH8JwVyBbWsEOVyZLcmRBsmC5do8eRGaNI7bOrbsQu2gXBW04t8yYaWqE5apoc?key=7ENonE7h1Ui3XJRQG3NJ9g" alt="" data-size="line"> Poisoned Training Data

* What it is: An attacker introduces malicious or biassed data into the large datasets used to train the LLM.
* Example: An attacker might subtly alter examples in a training dataset to introduce biases or include harmful content that the LLM might learn and reproduce.
* What it means: This can fundamentally affect the LLM's behaviour, leading to biassed outputs, generation of harmful content, or even the ability to trigger specific responses with hidden commands.

#### <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdFibualqw6SNKid9-NSR_KSC3rr1lq-CwUIeYyosSYd-5-RYA9hRymEk7TVT0MFhd7N2EKG44WQtEjvctJB2jk9ianjGricJ7PYDO4asTMLzVcIfqaNg4d1R6Rj9XwWsJowmRsHSFgl5pEA5E0mgEgvWoK?key=7ENonE7h1Ui3XJRQG3NJ9g" alt="" data-size="line"> Poisoned Fine-tune Data

* What it is: An attacker targets the smaller, specific datasets used to fine-tune the LLM for particular tasks or domains, injecting malicious or biassed data.
* Example: An attacker might submit manipulated data during a fine-tuning process to make the LLM less accurate, introduce specific biases, or generate harmful outputs in certain contexts.
* What it means: This can compromise the LLM's performance on specific tasks, introduce unwanted biases, or make it generate harmful content in targeted situations.

#### <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXeq7FCxpgrBafUNkAPWQkNCOaYVrs1i90BwzZsoMtto3pVZaQTV_C_k-_-DgL3Yrdo-XrQUZIAgGyczow5eru136ixd4Tyuc-HKS_welsFEWZ6_2KO6nbkUshfOKuWY4RYeqFxKr94QGkChsZw1n-Aegnb0?key=7ENonE7h1Ui3XJRQG3NJ9g" alt="" data-size="line"> Poisoned Memory

* What it is: An attacker manipulates the LLM's internal memory or state, potentially by exploiting vulnerabilities or through carefully crafted interactions.
* Example: An attacker might try to overload the LLM's memory with biassed information, inject malicious instructions, or disrupt its normal functioning.

What it means: This can lead to unpredictable behaviour, harmful outputs, or even a complete breakdown of the LLM's functionality.
