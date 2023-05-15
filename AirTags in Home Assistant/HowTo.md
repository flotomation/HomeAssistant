The local Cache on macOS is needed: ~/Library/Caches/com.apple.findmy.fmipcore/Items.data

Mac OS GUI APP FindMySync uses HA rest API to generate device_tracker entities:
https://github.com/MartinPham/FindMySync

Python Script and MQTT:
https://github.com/muehlt/home-assistant-findmy

Ruby Script and MQTT:
https://github.com/ndbroadbent/mac_airtag_to_mqtt


Run Mac OS (for testing) in KVM via Docker:
https://github.com/sickcodes/Docker-OSX

Notes for Docker:
Additional install requirements docker and podman
edit /etc/containers/registries.conf and add line: unqualified-search-registries = ["docker.io"]

run
sudo systemctl enable --now libvirtd

sudo systemctl enable --now virtlogd

echo 1 | sudo tee /sys/module/kvm/parameters/ignore_msrs

sudo modprobe kvm


For macOS Ventura erase disk with option HFS+ Journaled NOT APFS! You will run into errors



More on AirTags in Home Assistant:
https://community.home-assistant.io/t/is-there-any-way-to-track-apple-airtags-via-home-assistant/389049/32
