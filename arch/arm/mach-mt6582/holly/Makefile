
include $(srctree)/drivers/misc/mediatek/Makefile.custom

# Module project related part

ifeq ($(CONFIG_MTK_SENSOR_SUPPORT),y)
ifeq ($(CONFIG_MTK_EPL2182),y)
obj-y	+=  alsps/EPL2182/
endif

ifeq ($(CONFIG_MTK_TMD2771_HW_AUTO),y)
obj-y	+=  alsps/tmd2771_HW_auto/
endif

ifeq ($(CONFIG_MTK_BMA222E),y)
obj-y   +=  accelerometer/bma222E/
endif

ifeq ($(CONFIG_MTK_MMA8452Q_AUTO),y)
obj-y   +=  accelerometer/mma8452q_auto/
endif

ifeq ($(CONFIG_MTK_KX023_AUTO),y)
obj-y   +=  accelerometer/kx023_auto/
endif

ifeq ($(CONFIG_MTK_LIS3DH_AUTO),y)
obj-y   +=  accelerometer/lis3dh_auto/
endif

ifeq ($(CONFIG_MTK_AKM09911),y)
obj-y   +=  magnetometer/akm09911/
endif
endif

ifneq ($(CONFIG_ARCH_MTK_PROJECT),)
ARCH_MTK_PROJECT := $(shell echo $(CONFIG_ARCH_MTK_PROJECT))
obj-y	+= core/
obj-y	+= dct/dct/
endif

obj-y   +=  lcm/
#obj-y	+=  hdmi/
obj-y	+=  flashlight/
obj-y	+=  camera/camera/
#obj-y	+=  imgsensor/ov5648_mipi_raw/
#obj-y	+=  imgsensor/s5k4e1ga_mipi_raw/
#obj-y	+=  imgsensor/imx134liteon_mipi_raw/
#obj-y	+=  imgsensor/imx134sunny_mipi_raw/
obj-y	+=  vibrator/
obj-y	+=  leds/
obj-y	+=  keypad/
obj-y	+=  sound/
obj-y	+=  accdet/
obj-y	+=  partition/

