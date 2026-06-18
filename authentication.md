# API authentication

Authenticate API requests with a bearer token.

```bash
curl https://api.acmepay.example/v1/payments \
  -H "Authorization: Bearer test_api_key"
```

{% tabs %}
{% tab title="Node.js" %}
```javascript
const token = process.env.ACMEPAY_API_KEY;
```
{% endtab %}

{% tab title="Python" %}
```python
token = os.environ["ACMEPAY_API_KEY"]
```
{% endtab %}
{% endtabs %}
