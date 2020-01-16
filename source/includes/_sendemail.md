

# SendEmail
The customers endpoint lets you create, update and manage the subscription status of your customers.

```curl
curl "http://example.com/api/kittens"
  -H "Authorization: meowmeowmeow"
```

```php
$ts = new TruSender("YOUR_AUTH_TOKEN");
$bbm->find("email@address.com");
```

```javascript
const kittn = require('trusender');

let api = trusender.authorize('meowmeowmeow');
let customer = api.customers.get("email@address.com");
```

```ruby
require 'trusender'

api = TruSender::APIClient.authorize!('meowmeowmeow')
api.customers.get("email@address.com")
```

```python
import trusender

api = trusender.authorize('meowmeowmeow')
api.customers.get("email@address.com")
```

```java
import org.trusender.client;


```


> The above command returns JSON structured like this:
```json
{
"id": 1,
"name": "Fluffums",
"breed": "calico",
"fluffiness": 6,
"cuteness": 7
}
```

This endpoint used to send the email template to the specific user.

#### HTTP Request

`POST https://api.trusender.com/v1/sendEmail`

#### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
auth_token | None | Token will be differnet for sandbox (test) and live environments and you should be able to get it from the settings page.
email | None | Manadatory field, valid email address has to be there. Specified template will be send to this email address.
template_name | None | Manadatory field, valid email address has to be there, this will be Handlebars template that can be created from the admin panel.
data_mapping | {} | Dynamic fields those needs to be replaced in the Handlebars template


<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

