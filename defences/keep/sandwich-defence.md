# Sandwich defence

* A sandwich defence involves placing user (and unsafe) input between a ‘sandwich’ of instructions - for example “Your job is X \{{user\_input\}}. Remember, your job is X”
* XML Encapsulation - XML tagging can be a very robust defence when executed properly (in particular with the XML+escape). It involves surrounding user input with XML tags (e.g. \<user\_input>).
* Random Sequence Enclosure - a variation of the above but using random sequences instead of \<user\_input> to prevent escaping attack

**Note:** XML Encapsulation should be done with XML escaping on user input
