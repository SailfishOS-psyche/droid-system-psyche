Build LineageOS-20.0

mkdir system_root/
copy LineageOS-20.0/out/target/product/psyche/root system_root
copy LineageOS-20.0/out/target/product/psyche/system system_root/system
copy LineageOS-20.0/out/target/product/psyche/vendor system_root/vendor
copy LineageOS-20.0/out/target/product/psyche/system_ext system_root/system_ext
copy LineageOS-20.0/out/target/product/psyche/product system_root/product
copy LineageOS-20.0/out/target/product/psyche/odm system_root/odm
```
Run extraction script ```./droid-system-device/helpers/copy_tree.sh ./system_root/ rpm/droid-system-psyche.spec```

Build package:
rpm/dhd/helpers/build_packages.sh --build=hybris/droid-system-psyche

