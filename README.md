# onScreen Rails Gem

## Installation

Add this line to your application's Gemfile:

```ruby
    gem 'onScreen-rails'
```

And then execute:
```
    $ bundle install
```

## Usage

onScreen is dependant on jQuery, so make sure you have it in your Gemfile.

```
    //= require jquery
```

Add to your app/assets/javascripts/application.js

```
    //= require jquery.onscreen
```

Or for the minified version

```
    //= require jquery.onscreen.min
```


## Example
Include jQuery and the plugin on a page.

```html
$('elements').onScreen({
   container: window,
   direction: 'vertical',
   doIn: function() {
     // Do something to the matched elements as they come in
   },
   doOut: function() {
     // Do something to the matched elements as they get off scren
   },
   tolerance: 0,
   throttle: 50,
   toggleClass: 'onScreen',
   lazyAttr: null,
   lazyPlaceholder: 'someImage.jpg',
   debug: false
});
```

## Documentation

Usage documentation as well as demos can be found at:

http://silvestreh.github.io/onScreen/

https://github.com/silvestreh/onScreen
