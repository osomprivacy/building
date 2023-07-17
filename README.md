OSOM Privacy
============

The following instructions will allow you to sync and build the kernel for Solana Saga (ingot)

# Sync

```
repo init -u https://github.com/osomprivacy/building.git -b TKQ1.221220.425
```

# Build
```
EXT_MODULES="private/modules/uwb-stack/kernel private/modules/mmrm private/modules/datarmnet/core private/modules/datarmnet-ext/offload private/modules/datarmnet-ext/shs private/modules/camera/ private/modules/video/ private/modules/qcacld-3.0/ private/modules/audio/ private/modules/display/ private/msm-5.10/arch/arm64/boot/dts/vendor/qcom/audio private/msm-5.10/arch/arm64/boot/dts/vendor/qcom/camera private/msm-5.10/arch/arm64/boot/dts/vendor/qcom/display private/msm-5.10/arch/arm64/boot/dts/vendor/qcom/mmrm private/msm-5.10/arch/arm64/boot/dts/vendor/qcom/video private/modules/datarmnet-ext/aps/ private/modules/datarmnet-ext/perf private/modules/datarmnet-ext/perf_tether private/modules/datarmnet-ext/sch private/modules/datarmnet-ext/wlan private/modules/dataipa/drivers/platform/msm private/modules/cvp private/modules/eva private/modules/nfc" KERNEL_DIR=private/msm-5.10 BUILD_CONFIG=private/msm-5.10/build.config.msm.waipio VARIANT=gki build/build.sh
```
