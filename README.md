# ignition

My `.ign`-Files for CoreOS

## Generate ign-File

`docker run -i --rm quay.io/coreos/butane:release --strict < YAML.bu > JSON.ign`

## Use ign-File

```
curl -O https://raw.githubusercontent.com/realmiwi/ignition/master/JSON.ign
sudo coreos-installer install /dev/sda --ignition-file JSON.ign
poweroff
```
