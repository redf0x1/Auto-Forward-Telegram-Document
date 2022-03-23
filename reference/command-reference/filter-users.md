# Filter Users

{% hint style="info" %}
You can set a list of user id s to tell the bot to process messages you receive from source group only if it matches at least one of the user id's on the list.

🛑 **This feature work only for group**
{% endhint %}

{% tabs %}
{% tab title="Command" %}
Command Arguments\
`/filter_users ACTION LABEL LIST_USER_ID`
{% endtab %}

{% tab title="Example" %}
For Example

➡️ This will only allow messages from user\_id **123456** to be forwarded to **TARGET\_ID** with label **user1** \
`/filter_users add user1 123456`

➡️ This will only allow messages from user\_id **123456** or **565656** or **232323** to be forwarded to **TARGET\_ID** with label **user1** \
`/filter_users add user1 123456,565656,232323`

➡️ Remove list user with label **user1** \
****`/filter_users remove user1`

Show all filter users list \
****`/filter_users showall`
{% endtab %}
{% endtabs %}
