# cloudpayments-addons

Example:

```
http://www.yourhosthere.com?amount=123.12&description=Payment%20details&currency=RUB&invoiceId=123546&accountId=user@example.com
```

<ul>
<li>amount (required)</li>
<li>description (required) </li>
<li>currency (required)</li>
<li>invoiceId (required)</li>
<li>accountId (not required)</li>
</ul>

<h3>Make sure to define your Public ID and Success and Failure URLs</h3>

```
            // ID of your account
            const PUBLIC_ID = 'test_api_00000000000000000000001';
            // URL where the user gets redirected to after the successful transaction
            const SUCCESS_URL = 'http://www.google.com';
            // URL where the user gets redirected to after the failed transaction
            const FAILURE_URL = 'http://www.yahoo.com';
```

<h3></h3>
In case of successful or failed transaction, the user gets redirected either to SUCCESS_URL or FAILURE_URL respectively. The parameter "invoiceId" is added to the success and failure URL.
<h5>Example</h5>

```
            // URL where the user gets redirected to after the successful transaction
            const SUCCESS_URL = 'http://www.yoursite.com/success';
            // URL where the user gets redirected to after the failed transaction
            const FAILURE_URL = 'http://www.yoursite.com/failure';
```

In case when the transaction succeeded, the user gets redirected to

```
http://www.yoursite.com/success?invoiceId=12345
```

In case when the transaction failed, the user gets redirected to

```
http://www.yoursite.com/failure?invoiceId=12345
```
