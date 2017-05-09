# GeoMoose Desktop Testing Application

This demo is intended as a very basic starting point for an application.

The developers strive to provide a complete application without using a
given UI toolkit or Framework.  This version of the application provides
a grounds to demonstrate as many of the GeoMoose components as possible.

It is *preferable* to download one of the ready-made GeoMoose packages as
a starting point but it is certainly reasonable to fork and clone this repo.

## To Install (end users) ##

```
wget geomoose-demo-data.zip
wget geomoose-desktop-demo.zip
# apt-get install mapserver ?
# apt-get install apache ? nginx ?
# configure apache ? nginx ?
# 2. ?
# 3. Profit
```

## To Install (library developers) ##

```
  git clone geomoose/gm3
  cd gm3
  npm install
  grunt build
  glt clone geomoose/gm3-demo-data
  # "Magic to startup the docker instance here"
  git clone geomoose/gm3-demos
  cd gm3-demos/desktop
  ln -s ../../gm3 ./geomoose # or one could've just cloned in here, we would setup the gm3-demo-data .gitignore to just ignore "./geomoose" directories.
  npm install # installs a small web-proxying server.
  npm serve  # starts up a small webserver with a proxy to the demo data enabled.
 # And in another term...
 cd gm3
 npm install
 grunt build
 grunt watch # will do dynamic rebuilds w/ webpack.
```
