# Risk factors, outputs and attack vectors

### <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdl7oOEotfcXjPvSsb2h1GSuOK1VpOM3Ddcq2EORZOvXKEVXAnCvPRt2EH3XBRVhDdcUX8G29y3hY_Cf20ZySgvwJAhHOKBqq8Pi1Lw_L6FFFI1NbtarVLbZVgcttarm16ImpX7YB6yxvmmMqxN2rrxkrI?key=7ENonE7h1Ui3XJRQG3NJ9g" alt="" data-size="line"> Risk factors&#x20;

Risk factors are features and functionality within your LLM App which expose you to certain types of vulnerability. For example, if you provide user data to your LLM for it to make decisions, then you may be vulnerable to disclosing that data. On the other hand, if you never use proprietary data in training, for fine-tuning or retrieval augmented generation - there is no risk from exposing that data.

{% content-ref url="risk-factors.md" %}
[risk-factors.md](risk-factors.md)
{% endcontent-ref %}

#### <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd_AZ2ibaznyeuscLgKGEJoVjwRT6R4fWUkEumIlXSX64jTrXqMPvBUhFwRu3NKlb3r7XOlePA21J7Tflwb-tEXQgG9m71J4nkU7BiBiKTxR61_ZD9hYxSpOpkbizPkK0IpzfjGv-RujaJ6RKrwy_KcpBRm?key=7ENonE7h1Ui3XJRQG3NJ9g" alt="" data-size="line"> Outputs

Outputs are essentially what happens to the data produced by the model. This is important as if an attacker can never control the output for another user (e.g. because there is no memory or caching in place, no way of corrupting data etc) then there are no risks from XSS, also the risks associated with exposure of data do not exist if data is never sent to an attacker.&#x20;

{% content-ref url="outputs.md" %}
[outputs.md](outputs.md)
{% endcontent-ref %}

### <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXe4Gh6xS_lhbSqGs_ihT3ujxoVrPHEnUsX7XN1SwbNrLGz2KG7IMOrLDfqvgS40UTs3Se88YqCjSdg11bTkwJUl1omoxGzrqrgQ20CqJJfyKxvzoJ_6Ukxx4j1noJ2JmMmgvwqIvUX0AClEvOkec86Dqp6J?key=7ENonE7h1Ui3XJRQG3NJ9g" alt="" data-size="line">  Attack vectors&#x20;

Attack vectors are the mechanisms by which input can be tainted in such a way as to impact the correct functioning of an AI Application\


{% content-ref url="attack-vectors.md" %}
[attack-vectors.md](attack-vectors.md)
{% endcontent-ref %}

