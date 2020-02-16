# Setup Instructions

## Download / Install Docker
    https://www.docker.com/products/docker-desktop

## Clone Repo
    git clone https://github.com/MBahrSNC/snDockerMID.git
    cd snDockerMID

## Build Image
    docker build -t snmid .

## Build Container 
    Replace <ENTER INSTANCE URL>, <ENTER INSTANCE USERNAME>, <ENTER INSTANCE PASSWORD>, <ENTER MID SERVER NAME>


## Example
    docker run -d --name snmid -e 'SN_URL=https://dev12345.service-now.com' -e 'SN_USER=admin' -e 'SN_PASSWD=supersecret' -e 'SN_MID_NAME=snDockerMID' snmid:latest

## Run
    docker run -d --name snmid -e 'SN_URL=<ENTER INSTANCE URL>' -e 'SN_USER=<ENTER INSTANCE USERNAME>' -e 'SN_PASSWD=<ENTER INSTANCE PASSWORD>' -e 'SN_MID_NAME=<ENTER MID SERVER NAME>' snmid:latest

