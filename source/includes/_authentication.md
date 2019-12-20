
# Authentication

> To authorize, use this code:

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
```

```shell
# With shell, you can just pass the correct header with each request
curl "api_endpoint_here"
  -H "Authorization: meowmeowmeow"
```

```javascript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
```

> Make sure to replace `meowmeowmeow` with your API key.

To authenticate against the Vero API, you need to use your auth_token in each request. Your `auth_token` can access all of your data and, with future API releases, will be able to read from Vero too. Ensure you keep it secret!

To access your API credentials, visit the [Settings] (https://www.google.com) page within your TruSender account.

Requests are authenticated by providing a parameter called auth_token containing your `auth_token` with each request.

All API requests must be made over HTTPS. Calls made over plain HTTP will fail. You must authenticate for all requests.

<aside class="notice">
You must replace <code>meowmeowmeow</code> with your personal `auth_token`.
</aside>