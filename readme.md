THEA-LOCAL_MANIFEST
========================
Project for motorola Moto G 2014 LTE (THEA)

### Installing Repo ###
```bash
# Make a directory where Repo will be stored and add it to the path
    $mkdir ~/.bin
    $PATH=~/.bin:$PATH

# Download Repo itself
    $curl https://storage.googleapis.com/git-repo-downloads/repo > ~/.bin/repo

# Make Repo executable
    $chmod a+x ~/.bin/repo
```

### Initializing Repo ###
```bash
    $ repo init -u git://github.com/CyanogenMod/android.git -b cm-12.1
    $ curl --create-dirs -L -o .repo/local_manifests/roomservice.xml -O -L https://raw.githubusercontent.com/RolanDroid/local_manifest/cm-12.1/roomservice.xml
```
### For sync: ###
```bash
    $repo sync -j4
```
### To build for your device.. ###
```bash
    $ build/envsetup.sh
    $ breakfast device_name_here
    $ brunch device_name_here
```


