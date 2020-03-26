SMS Counter
=============================

Character counter for SMS messages.


Usage
----------

```javascript
SmsCounter.count('content of the SMS')
```

This will return the following object:

```javascript
{
	encoding: "GSM_7BIT",
	length: 18,
	messages: 1,
	per_message: 160,
	remaining: 142
}
```

jQuery Plugin
----------

Given the following markup:

```html
<textarea name="message" id="message"></textarea>
<ul id="sms-counter">
	<li>Encoding: <span class="encoding"></span></li>
	<li>Length: <span class="length"></span></li>
	<li>Messages: <span class="messages"></span></li>
	<li>Per Message: <span class="per_message"></span></li>
	<li>Remaining: <span class="remaining"></span></li>
</ul>
```

You can use the `countSms` jQuery extension to update the count on keyup:

```javascript
$('#message').countSms('#sms-counter')
```


TODO
----

- Better docs


Known Issue
----

(none)


Other Languages
----

- PHP: [https://github.com/acpmasquerade/sms-counter-php](https://github.com/acpmasquerade/sms-counter-php)
- C#: [https://github.com/troll31/sms-counter-csharp](https://github.com/troll31/sms-counter-csharp)


## License

SMS Counter is released under the [MIT License](LICENSE.txt).