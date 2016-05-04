# RailsConf 2016

## Stuck in the Middle: Leverage the power of Rack Middleware

http://www.whynot.io/ruby/what-is-rack-in-ruby/

Rack sets "environment" hash

3 parts:
- Handler takes care of WEBrick
- Adapter talks to framework
- Middlewares work with request/response as it passes through stack
    + used in rails to setup cookies, flash messages, logging, and params parsing

rack-throttle on github

Middleware can deal with requests your app should never worry about
- can be protective
- sees request and response
- easily extracted to shareable tool

Middlewares run in a certain order
`rake middleware`

Doesn't belong in middleware:
- modifying the request
- knows about business logic in the app
- knows about models in the app

Always return a response
@cdwort