Trelfred
========

An experimental [Alfred][] Workflow for quickly visiting [Trello][] boards.

[Alfred]: http://www.alfredapp.com/
[Trello]: https://trello.com/

Ruby Version
------------

The workflow currently requires that you specify the ruby version. This is done
by including the RVM intialization line before executing the script. If you
use an alternate ruby switcher, these references must be changed to properly
initialize your ruby version tool.

In addition, the following gems must be installed for the ruby the script will
run with:

- [Dotenv][]
- JSON
- [Nokogiri][]
- [String Score][]
- [RestClient][]

[RestClient]: https://github.com/rest-client/rest-client
[String Score]: https://github.com/jlindley/string_score_ruby
[Dotenv]: https://github.com/bkeepers/dotenv
[Nokogiri]: http://nokogiri.org/

Credentials
-----------

Trelfred expects credentials be exposed in a `~/.env` file. The file should have
the following structure / keys:

``` env
TRELLO_USERNAME=ctoomey
TRELLO_DEVELOPER_KEY=14363e6563fea5ace63d6f
TRELLO_TOKEN=0fd4c5bbab47cc9c2b81dcbedaf28061a1ac0934f14c7475af8857b76de96b99
```

### TRELLO DEVELOPER KEY

You can generate this key by visiting [here](https://trello.com/1/appKey/generate)

### TRELLO TOKEN

You can generate this key by visiting the following URL (**note** you will have
to replace the developer token in this URL):

https://trello.com/1/authorize?key=substitutewithyourapplicationkey&name=Trelfred&expiration=30days&response_type=token

You can find more detail in the Trello API Documentation - [Generating a Token
from a User][] section.

[Generating a Token from a User]: https://trello.com/docs/gettingstarted/index.html#getting-a-token-from-a-user
