# OmniAuth Social Stream

This is the official OmniAuth strategy for authenticating to a Social Stream node
that includes the [Social Stream OAuth2 Server gem](https://github.com/ging/social_stream/oauth2_server). To use it, you'll need to sign up for an OAuth2 Application ID and Secret
on the Social Stream node. There is an example in [Social Stream's demo site](http://demo-social-stream.dit.upm.es).

## Usage

    provider :social_stream, ENV['SS_KEY'], ENV['SS_SECRET'],
        {
          :client_options => {
            :site => 'https://demo-social-stream.dit.upm.es/api',
            :authorize_url => 'https://demo-social-stream.dit.upm.es/login/oauth/authorize',
            :token_url => 'https://demo-social-stream.dit.upm.es/login/oauth/access_token',
          }
        }

## License

Copyright (c) 2013 Universidad Politécnica de Madrid

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
