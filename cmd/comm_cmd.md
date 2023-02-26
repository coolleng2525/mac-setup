


# root dir

## this need root priv
sudo mount -uw /
sudo mkdir -p /data




## macOS Catalina, mkdir path
sudo mkdir -p /System/Volumes/Data/data/db

## give permissions
sudo chown -R `id -un` /System/Volumes/Data/data/db

## macOS 10.14.x -
sudo mkdir -p /data/db

## macOS 10.15.x +
sudo mkdir -p /System/Volumes/Data/data/db

