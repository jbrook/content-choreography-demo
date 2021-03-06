# Content Choreography #

This is my attempt at responsive [content choreography](http://www.jordanm.co.uk/post/21863299677/building-with-content-choreography) as described by Jordan Moore in his [excellent article](http://www.jordanm.co.uk/post/21863299677/building-with-content-choreography
). He has a good [demo](http://www.jordanm.co.uk/lab/contentchoreography) too.

In short, we can have a different layout order when the content is displayed in a 'small context'. In my case the 'small context' is the default because I have tried to implement this 'mobile first'.

As in Jordan's demo, the content re-ordering is achieved using [CSS flexbox](http://www.w3.org/TR/2009/WD-css3-flexbox-20090723/), which has wide support amongst common 'mobile' browsers. However in the 'larger contexts' we switch to using standard "block" display. Note that this is using the 2009 spec and not the more recent 2012 version.

In the larger contexts this example makes use of a fluid and responsive CSS grid generated by the ["susy" SASS plugin for Compass](http://susy.oddbird.net). I realise that all of my content is the same width in a single column but I intend to play with grids at some point too.


## Typography Stuff ##

I learnt something about [vertical rhythm](http://typecast.com/blog/4-simple-steps-to-vertical-rhythm) and [modular scale](http://www.alistapart.com/articles/more-meaningful-typography/). This demo integrates a compass extension for each with a [SASSified version of normalize.css](https://github.com/JohnAlbin/normalize.css-with-sass-or-compass) stolen from JohnAlbin.


## Disclaimer ##

This is the first time I have ever really done anything with CSS or SASS. I have copied and pasted a lot of this. Just playing...


## Dependencies ##

    gem install sass
    gem install compass
    gem install susy
    gem install modular-scale