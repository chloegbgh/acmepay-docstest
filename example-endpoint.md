# Example endpoint

Create a payment.

```http
POST /v1/payments
Content-Type: application/json
```

```json
{
  "amount": 2500,
  "currency": "eur",
  "customer_id": "cus_demo_123"
}
```

Expected response:

```json
{
  "id": "pay_demo_456",
  "status": "succeeded"
}
```
