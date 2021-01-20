# recaptcha-sitekeys

A list of reCAPTCHA settings and site keys of different websites. Mainly used
by [decaptcha](https://github.com/schnusch/decaptcha).

[sitekeys.json](sitekeys.json) contains an object according to [schema.json](schema.json).
For example it might look like this:

```json
{
	"decaptcha.test": {
		"sitekey": "6LeIxAcTAAAAAJcZVRqyHh71UMIEGNQ_MXjiZKhI",
		"invisible": true,
		"hosts": ["decaptcha2.test"]
	}
}
```

Only the `sitekey` property is mandatory, `hosts` is a list of hosts for which
these settings are also valid.

There is also a simplified version:

```json
{
	"decaptcha.test": "6LeIxAcTAAAAAJcZVRqyHh71UMIEGNQ_MXjiZKhI"
}
```

which should be equivalent to this:

```json
{
	"decaptcha.test": {
		"sitekey": "6LeIxAcTAAAAAJcZVRqyHh71UMIEGNQ_MXjiZKhI"
	}
}
```
