<h2>Create an Image using Dockerfile</h2>
```docker
FROM busybox
WORKDIR /usr/src/app
COPY . .
CMD find . -print | sort | sed 's;[^/]*/;|---;g;s;---|; |;g'
```

<h2>Build the Image</h2>
```
docker build -t build-context
```

<h2>Run the Container</h2>
```
docker run --rm -it build-context
```

You will get the complete file structure, then you can manipulate it.