# Nativescript + SASS Animations
This is a Nativescript & SASS port of the popular [animate.css](https://github.com/daneden/animate.css) library for your Nativescript + SASS apps.

## How To
* Install. (Its expected that you have nativescript-dev-sass installed as well). 
```
npm i nativescript-animate-sass --save
```

* In your SASS file.
``` scss
@import '~nativescript-animate-sass';

.pulse {
  @include pulse(2.5s, ease-in, true);
}
```

This should produce
``` css
.pulse { 
  animation-name: pulse;
  animation-duration: 2.5s;
  animation-fill-mode: both;
  animation-timing-function: ease-in;
  animation-iteration-count: infinite;
}
```

* In your Component. 
``` html
  <Button class="pulse" text="Animate"></Button>
```

* Thats all. For more info on animations, see [animate.css](https://github.com/daneden/animate.css).

## License

[MIT](/LICENSE)
