# fastroads

This is a modded version of [slowroads.io](slowroads.io) that adds two fast cars and some other stuff. I did not make the original game. The original game is at [slowroads.io](slowroads.io), and it was created by [anslo](https://twitter.com/anslogen). Unfortunately the cars in the original game are too slow and he did not make the source code public, so all we have to work with is the minified JS. Some notes:

- There is now a "Lambo" that can reach speeds of about 363 mph. It looks the same as the roadster and doesn't handle too well but it's fun
- There is a "Supercar" that can reach speeds up to about 6000 mph. It looks like the roadster as well and handles as well as a 6000 mph car can
- In addition to the three difficulties ("casual", "normal", "hard") there is now "wide" and "straight." "Wide" generates wider roads, and "straight" generates a straight, flat, wide road.
- There is a graphics option called "ultra+" that increases the render distance. Unfortunately using ultra+ disables tree generation entirely and I'm not sure why.

# Running

The files in this repo were obtained by just saving whatever was served up by slowroads.io, so you need a local http server to run this. You can use `http-server` from npm. To do this you will first need nodejs. Once you have nodejs installed, run

```sh
npm i -g http-server
```

to install `http-server` globally. Then `cd` into the repo and run

```sh
http-server
```

to start the server. `http-server` will print the address to connect to - this will probably be something like `http://127.0.0.1:8081`. Visit this address in your browser to play the game. If you change a file, CTRL + F5 will invalidate the cache and reload the entire page.

# Contributing

Any contributions are welcome. I am working on improving the handling of the new cars and giving them textures as well as fixing the ultra+ bug. I am also naming minified variables as I figure out what they mean.
