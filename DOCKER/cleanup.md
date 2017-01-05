#### Docker is a garbage generating machine.  After some time, you'll want to clean up dangling images.
Snippet from from [Open edX on Docker Wiki](https://openedx.atlassian.net/wiki/display/OpenOPS/Open+edX+on+Docker#suk=)
> docker rmi $(sudo docker images -f "dangling=true" -q)

#### After some time, you'll want to clean up dangling volumes.
> docker volume rm $(docker volume ls -qf dangling=true)

#### Delete Containers that are not running
Start the docker host (without using their quickstart scripts) on OSX
bash --login /Applications/Docker/Docker\ Quickstart\ Terminal.app/Contents/Resources/Scripts/start.sh
