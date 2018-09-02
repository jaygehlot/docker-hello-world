A very basic Docker Hello World

Using Denbian Linux distribution, running apache and php. 

Port 80 is exposed on the Image, so when running the container using (where hello-world is the name of the container)

```
docker run -p 80:80 hello-world
```

Or to mount a volume (this allows immediates changes made to the php file to be shown, it effectively lets you share files/folders between your host, and your running container, you can mount a folder inside your host, then when you are running the container, if you change files on your host, which have been mounted, you can see the changes instantly on your container ---- this will give a live view of the file changes 
when calling localhost:80 )

```
docker run -p 80:80 -v <location of src folder>:/var/www/html hello-world
```

Created watching https://www.youtube.com/watch?v=YFl2mCHdv24
