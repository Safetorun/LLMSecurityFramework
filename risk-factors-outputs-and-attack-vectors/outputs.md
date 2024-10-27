# Outputs

#### <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXd_AZ2ibaznyeuscLgKGEJoVjwRT6R4fWUkEumIlXSX64jTrXqMPvBUhFwRu3NKlb3r7XOlePA21J7Tflwb-tEXQgG9m71J4nkU7BiBiKTxR61_ZD9hYxSpOpkbizPkK0IpzfjGv-RujaJ6RKrwy_KcpBRm?key=7ENonE7h1Ui3XJRQG3NJ9g" alt="" data-size="line">Outputs

Outputs are essentially what happens to the data produced by the model. This is important as if an attacker can never control the output for another user (e.g. because there is no memory or caching in place, no way of corrupting data etc) then there are no risks from XSS, also the risks associated with exposure of data do not exist if data is never sent to an attacker.&#x20;

#### <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXe9Jeen8kEfNBD7Qrwp5iSK9J6hrrRL23sKUqoPXmS-rFy5Fy5VesmcmyMnmHh8PnLBBEsiWtKvjfxYDs0y9nZWFzOhxm9jeb-k0gofCzgqjNTPwhLQ8MT2krrJMHMq7tGjFrflq4-S2-T9HylZIQDOnRCx?key=7ENonE7h1Ui3XJRQG3NJ9g" alt="" data-size="line"> To Attacker

This is where output from an LLM can be sent to an attacker. There are many examples of this - for example in a chatbot output sent to an attacker. On the other hand, there are examples where this is not the case - AI used in filtering spam would not present data back to a user.

#### <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXel4Izuu3Y_5VJ4x-RQU5SKcPQ2nmSW-DSw7MtIacgP2CDSubyk8D1wYfd0PHVrqqQNKl1426vU8ipZIs1lm8on_F6BGxzsEPatbFGemYWOLsZQ-abUKpo57pnmw3ejf0INvAcHbF1TdGRn9BDeKiew6kK3?key=7ENonE7h1Ui3XJRQG3NJ9g" alt="" data-size="line"> To User

This is where output of an LLM can be sent to a user. Consider in these cases where data is sent via indirect means (for example an email) as well as the response being directly rendered in a web or mobile app.

#### <img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfnUPmR37Sl63NCB8_6ErGrIsAYIgb0C61irdaqowBdgNC5anyD-ZZrbMrrtjLkH7vodBzTT5-UTYxTFUW8TklTvyN90gf1DZgorkP99jeUEpPWPAKJiRp5sG-C2XfwKUy8qfY-mGI047hkrdd0OWzMJpKv?key=7ENonE7h1Ui3XJRQG3NJ9g" alt="" data-size="line">Decision making&#x20;

This is where an LLM’s output is used to make a decision - these are common in things like CV filtering apps, spam filters and fraud detection platforms.

\
