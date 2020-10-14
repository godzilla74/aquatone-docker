Forked from: https://github.com/youngderekm/aquatone-docker but had to make some modifications to the Dockerfile to get
things to work correctly.

Get started with:
```
git clone git@github.com:godzilla74/aquatone-docker.git
```

Then you'll probably want to modify this line:
```
vim Dockerfile
---> change ENV TZ=Whatever
```

Then build it and run:
```
sudo docker build -t aquatone .

cat your_domain_file | sudo docker run -v /where/to/output:/output --rm -i aquatone:latest -out /output
```
