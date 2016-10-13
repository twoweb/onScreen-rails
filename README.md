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
var os = new OnScreen({
  tolerance: 0,
  debounce: 100,
  container: window
});

// Do something when an element enters the viewport
os.on('enter', '.someCSSSelector', (element) => {
  // makes's the element's text red
  element.style.color = 'red';
});

// Do something else when an element leaves
os.on('leave', '.someCSSSelector', (element) => {
  // makes's the element's text black
  element.style.color = 'black';
});
```

## Documentation

Usage documentation as well as demos can be found at:

http://silvestreh.github.io/onScreen/

https://github.com/silvestreh/onScreen
