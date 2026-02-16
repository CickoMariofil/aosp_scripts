# aosp_scripts

```
lunch voltage_fuxi-bp4a-userdebug
breakfast device (fuxi) - preparation
brunch device (fuxi) - building zip
```

Helper scripts

Target release is found in build/envsetup.sh
```
make clobber
source build/envsetup.sh
```

Add additional lunch choices in device/XX/AndroidProducts.mk as: 

```
COMMON_LUNCH_CHOICES := \
lineage_lilac-ap2a-user \
lineage_lilac-ap2a-userdebug \
lineage_lilac-ap2a-eng
```

lilac – device codename, ap2a- target release from envsetup


```
#export TARGET_RELEASE=ap2a
lunch
lunch aosp_cf_x86_64_phone-ap2a-eng
#build_build_var_cache
#lunch
make bacon - recovery .zip 
```

## 
Target release is found in build/envsetup.sh
make clobber
source build/envsetup.sh
source vendor/voltage/vendorsetup.sh

vendor/voltage-priv/keys

Add additional lunch choices in device/XX/AndroidProducts.mk as: 

COMMON_LUNCH_CHOICES := \
lineage_lilac-ap2a-user \
lineage_lilac-ap2a-userdebug \
lineage_lilac-ap2a-eng

lilac – device codename, ap2a- target release from envsetup


#export TARGET_RELEASE=ap2a
lunch
lunch aosp_cf_x86_64_phone-ap2a-eng
#build_build_var_cache
#lunch
make bacon

lunch voltage_fuxi-bp4a-userdebug

breakfast device
brunch device

payload dumper – fw
mount : sudo mount -r system.img system/
mount other (vendor, odm, product, system_ext) the same way but to system/vendor (etc) folders

./extract_files.sh from system/ folder

copy radio module imgs (proprietary firmware files) to corresponding folder
vendor/xiaomi/fuxi/radio
sudo cp modem.img /run/media/mario/andro/fuxi/los16/vendor/xiaomi/fuxi/radio/modem.img

./setup_makefiles.sh

brunch device
