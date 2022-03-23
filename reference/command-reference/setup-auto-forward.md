# Setup Auto Forward

{% hint style="warning" %}
This command is used for setting up auto forward. This command should be run after you have already connected a telegram account with [connect](connect-phone.md) command.
{% endhint %}

{% embed url="https://www.youtube.com/watch?v=p3KDSrinlsA" %}
How to get chanel id, group id, chat id telegram
{% endembed %}

{% embed url="https://www.youtube.com/watch?v=umCVIHbO-SU" %}
How to create forward task
{% endembed %}

{% hint style="info" %}
#### &#x20; Command Information

* This commands needs input from the **** /getchanel or /getgroup or /getuser
* You can only use source and target id's you find via /getchanel or /getgroup or /getuser
* **LABEL** is the nickname you want to give to your setup. Do not use numbers you get from /getchanel or /getgroup or /getuser in this field or Telegram chat names. This variable is used to define a nickname so you can identify your setup later on every **Auto Forward Telegram BOT** command.
{% endhint %}

{% tabs %}
{% tab title="Command" %}
**Use the following syntax for adding channels/users/bots:**\
`/forward [ACTION] [LABEL] [SOURCE_CHAT_ID] -> [TARGET_CHAT_ID]`
{% endtab %}

{% tab title="Example" %}
**One to One**\
`/forward add work1 22222 -> 66666`\
\
**Many to One**\
`/forward add work1 22222,33333 -> 66666`\
\
**One to Many**\
`/forward add work1 22222 -> 66666,77777`\
\
**Many to Many**\
`/forward add work1 22222,33333 -> 66666,77777`\
\
\===============\
\
**Remove task with label work1 in list**\
`/forward remove work1`\
\
**Start task with label work1 in list**\
`/forward start work1`\
\
**Stop task with label work1 in list**\
`/forward stop work1`\


**Set delay 30 seconds to each message with label work1** \
`/forward delay work1 30`\


**Set maximum time limit to receive message edit event from SOURCE\_ID is 30 seconds with label work1** \
`/forward max_time_edit work1 30`

\
**Restart all process if any error**\
`/forward restart`\
\
**Show all list task**\
`/forward task`
{% endtab %}
{% endtabs %}

{% hint style="danger" %}
&#x20; **Syntax Limitations**

* ID's can only be numbers
* You can only use **->** once
* You should never repeat the same setup
* You should never use the **same ID** in both **source** and **target**
{% endhint %}
