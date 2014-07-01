UK Cinema Listing/Rating App
====
This simple webapp lets you see film listings with inline ratings for Cineworld and Odeon cinemas. You can [see it in action here](http://gregd.me/cineworld/).

Getting Started
====
Running locally
----
It's a simple self contained webapp using relative paths, so you just need to host it with a webserver.

My approach is:
cd src
python -m SimpleHTTPServer

You can then go to http://localhost:8000 and see the app.

However, it attempts to connect to a locally running copy of my cinema-service backend. So, for local testing I have a mocked out movie service - take a look at DummyMovieService and RealMovieService in films.html - it's fairly straightforward.

Making Changes
----
The site isn't too complex. No real frameworks - just jQuery for ajax, Polymer/Web Componentsfor for the view, and Finch for routing.

I've deliberately (read: lazily) avoided anything that needs a pre-processer such as typescript and sass (both of which are cool - and I may start using here). I am using bower though - but the bower components are all committed and you can just ignore it if you wish. :)


License (GPLv3)
----
Copyright (c) Greg Dorrell

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.
