include $(TOPDIR)/rules.mk

ARCH:=aarch64
BOARD:=ipq60xx
BOARDNAME:=Qualcomm Atheros IPQ60xx
FEATURES:=squashfs fpu ramdisk nand
MAINTAINER:=John Crispin <john@phrozen.org>
CPU_TYPE:=cortex-a53
SUBTARGETS:=generic

KERNEL_PATCHVER:=4.4

KERNELNAME:=Image dtbs

include $(INCLUDE_DIR)/target.mk
DEFAULT_PACKAGES += \
	kmod-leds-gpio kmod-gpio-button-hotplug swconfig \
	nss-firmware-ipq6018 kmod-qca-nss-dp kmod-qca-nss-ecm \
	kmod-ath11k-ahb wpad-openssl ath11k-firmware-ipq6018 \
	kmod-qca-ssdk qca-ssdk-shell kmod-qca-nss-drv \
	kmod-qca-nss-drv-pppoe kmod-qca-nss-drv-bridge-mgr \
	autocore-arm luci-app-cpufreq uboot-envtools

$(eval $(call BuildTarget))
