# local-cache
LocalCache

imported from Google Code project
https://code.google.com/p/local-cache/

I'm not the author, but just wanted to save the script when Google Code shuts down

#The original ReadMe

With HTML 5 we get localStorage, which is a quick & easy way for storing name/value pairs locally. However, unlike with cookies, we do NOT get the ability to expire items that we set in localStorage.

This extension provides just that: setting items in localStorage that expire when you tell them to.

Example: <code>localStorage.setCacheItem("usersFavoriteColor", "blue", { days: 1 });</code>

The above expires in 1 day, as long as you retrieve that item using the following:

<code>var color = localStorage.getCacheItem("usersFavoriteColor");</code>

which will return null if it has expired.

Please note: you can store/retrieve json objects directly, without any stringify'ing or parsing.

Example: <code>localStorage.setCacheItem("usersFavoriteCar", { year: 2012, make: "Honda", model: "Civic" }, { years: 1 });</code>

then to retrieve it...

var car = localStorage.getCacheItem("usersFavoriteCar"); alert(car.year);

Feedback? Yes please! Please submit via the Issues tab.

Want to download? Please click on the Downloads tab.
