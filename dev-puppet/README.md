# dev-puppet
some basic containers to do practice puppet

## how it's supposed to work (but doesn't atm)
`docker-compose up --build`
and bam, master-agent setup to play with

## stuff that actually works:
`docker build -f Dockerfile.puppetserver -t dev-puppetserver .`
`docker run -it dev-puppetserver bash`
