# aosp_scripts
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
