# Carthage dependencies

In order to build Carthage dependencies with Xcode *BEFORE* 12, run the following command from terminal:

```sh
> carthage update --no-use-binaries --platform iOS
```

In order to build Carthage dependencies with Xcode *FROM* 12 onwards, run the following command from terminal:

```sh
> ./carthage-xc12.sh update --no-use-binaries --platform iOS
```

# Sample images for testing

In order to successfully build and run tests and sample apps, some (large) images are needed
which are not included under source control and thus must be downloaded separately. 

* SwiftyGifTests/Images/sample.jpg  
  This has been removed in commit [c804e36](https://github.com/kirualex/SwiftyGif/commit/c804e36ea21f25715a55216ff40d18c3941f8ced) 
  and so it can be restored from its parent commit

* SwiftyGifTests/Images/15MB_Einstein_rings_zoom.gif  
  This can be downloaded from [wikimedia](https://commons.wikimedia.org/wiki/File:Einstein_rings_zoom.gif) 
  and renamed as `15MB_Einstein_rings_zoom.gif`
