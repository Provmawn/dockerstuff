# dev-golang
basic golang container to test golang stuff

## stuff that works
`docker build -t dev-golang -f Dockerfile.golang .`

WINDOWS
`docker run -it -v ${pwd}:/usr/local/src dev-golang`


LINUX
`docker run -it -v $(pwd):/usr/local/src dev-golang`

## stuff that doesn't work
the docker-compose script doesn't work because container ends and returns 0

am pretty sure i have to do ${pwd} or $(pwd) depending on the OS too in the docker-compose