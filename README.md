mailchimp-webhooks
==================

Allows a WordPress site to act as a MailChimp webhook.

Plugin will toggle a new user meta variable, _newsletter_subscriber, when a user subscribes or unsubscribes from a MailChimp list 
or will, optionally, add new subscribers and delete unsubscribers.

The URL listed in the plugin's settings page needs to be used when configuring the webhook in MailChimp.


usage
==================
Create a config.php which includes the defination of

```
MCWH_LIST_IDS
```

which is a map from mailchimp list id to user_meta_data prefix,

and

```
COMMON_TAGS
```

which is a map from mailchimp field to user_meta_data field name.
