# cloudpayments-addons

Example:
```
http://www.yourhosthere.com?amount=123.12&publicId=test_api_00000000000000000000001&description=Payment%20details&currency=RUB&invoiceId=123546&accountId=user@example.com&successUrl=http://www.google.com&failureUrl=http://www.yahoo.com
```

<ul>
<li>amount (required)</li>
<li>publicId (required) </li>
<li>description (required) </li>
<li>currency (required)</li>
<li>invoiceId (not required)</li>
<li>accountId (not required)</li>
<li>successUrl (required) - URL, where the user gets forwarded to after the successful transaction</li>
  <li>failureUrl (required) - URL, where the user gets forwarded to after the failed transaction</li>
</ul>
