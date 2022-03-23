# Replace

{% hint style="info" %}
You can set a list of words or regex patterns which tells the bot that if the message received from source channel has any of the replace words or regex pattern match the bot should replace that message with the word you want to change.
{% endhint %}

{% hint style="danger" %}
This feature will not work if you enable "**Show Forward Headers**" in task list
{% endhint %}

{% tabs %}
{% tab title="Command" %}
➡️ Command Arguments\
`/replace ACTION LABEL Original_WORD -> NEW_WORD`\
\
➡️ USE Regex\
`/replace ACTION LABEL_regex Regex_syntax -> NEW_WORD`
{% endtab %}

{% tab title="Syntax Example ( Simple )" %}
Use the syntax as shown below when you want to replace words or full paragraphs.\
\
➡️ Change **black** to **white**\
**`/replace add re1 black -> white`**

➡️ Remove keyword **black** from the message\
`/replace add re1 black -> EMPTY`
{% endtab %}

{% tab title="Syntax Example ( Advanced )" %}
{% hint style="info" %}
Use the syntax as shown below when you want to achive result that is not possible with the simple syntax. This syntax uses regex to replace words and keywords and you can do everything you want with the message if you know regex.
{% endhint %}

{% hint style="warning" %}
**We do not support usage of regex, you are on your own if you decide to use regex. Only use it if you know what you are doing.**
{% endhint %}

➡️ Change **good** or **perfect** to **bad**\
****`/replace add re1_regex (good|perfect) -> bad`

➡️ Match every **url** or **@mention** and change it to @Auto\_Forward\_Messages\_Bot \
\`/replace add re1\_regex (@|www|https?)\S+ -> @Auto\_Forward\_Messages\_Bot
{% endtab %}
{% endtabs %}

