# dev-puppet
some basic containers to do practice puppet

## how it's supposed to work (but doesn't atm)
`docker-compose up --build`
and bam, master-agent setup to play with

## useful stuff that actually works:
`docker build -f Dockerfile.puppetserver -t dev-puppetserver .`

`docker run -it --rm -v $(pwd):$(pwd) -w $(pwd) dev-puppetserver bash`

`for i in *.pp; do puppet parser validate $i; done`

