# Rack

## Spec

A Rack application is an Ruby object (not a class) that responds to `call`. It takes exactly one argument, the environment and returns an Array of exactly three values: The status, the headers, and the body.

## A Tiny Example

```ruby
require 'rubygems'
require 'rack'

class HelloWorld
  def call(env)
    [200, {"Content-Type" => "text/html"}, "Hello Rack!"]
  end
end

Rack::Handler::Mongrel.run HelloWorld.new, :Port => 9292
```

## Rack::Builder

*rackup* converts your config script to an instance of `Rack::Builder`.

```ruby
infinity = Proc.new {|env| [200, {"Content-Type" => "text/html"}, env.inspect]}
builder = Rack::Builder.new do
  use Rack::CommonLogger
  run infinity
end
Rack::Handler::Mongrel.run builder, :Port => 9292
```

## Refs

* http://m.onkey.org/ruby-on-rack-1-hello-rack
* http://m.onkey.org/ruby-on-rack-2-the-builder