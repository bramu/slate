

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

This endpoint retrieves all kittens.

### HTTP Request

`GET http://example.com/api/kittens`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
include_cats | false | If set to true, the result will also include cats.
available | true | If set to false, the result will include kittens that have already been adopted.

<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

