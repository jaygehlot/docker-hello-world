A very basic Docker Hello World

Using Denbian Linux distribution, running apache and php. 

Port 80 is exposed on the Image, so when running the container using (where hello-world is the name of the container)

```
docker run -p 80:80 hello-world
```

Or to mount a volume (this allows immediates changes made to the php file to be shown
when calling localhost:80

```
docker run -p 80:80 -v <location of src folder>:/var/www/html hello-world
```

Created watching https://www.youtube.com/watch?v=YFl2mCHdv24
