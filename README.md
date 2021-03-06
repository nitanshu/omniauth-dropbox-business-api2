OmniAuth Dropbox Business API 2
=====================================

Strategy to authenticate Dropbox in OmniAuth using the business api v2.

It's using the OAuth2 from the [Dropbox API](https://www.dropbox.com/developers) Business EndPoint.

Usage
-----

Add the strategy to your `Gemfile` alongside OmniAuth:

```ruby
gem 'omniauth-dropbox-business-api2'
```

Integrate this strategy to your OmniAuth middleware.

```ruby
use OmniAuth::Builder do
  provider :dropbox_oauth2, ENV['DROPBOX_KEY'], ENV['DROPBOX_SECRET']
end
```

You need to add your key and secret.

Also remember to add the full callback path to your Dropbox App Console, for example: https://example.com/auth/dropbox_oauth2/callback

For more information check the [OmniAuth wiki](https://github.com/intridea/omniauth/wiki).


Helping
-------

* Fork the project, make your changes and send me a pull request.
* Create an issue! :D

License
-------

Copyright (c) 2017 Nitanshu Verma

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
