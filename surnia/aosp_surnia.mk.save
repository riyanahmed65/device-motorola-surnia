#
# Copyright (C) 2015 The Android Open-Source Project
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#

# Inherit from surnia device
$(call inherit-product, device/motorola/surnia/device.mk)

# Inherit some common stuff.
$(call inherit-product-if-exists, vendor/aosp/config/common_full_phone.mk)

# Boot animation
TARGET_BOOT_ANIMATION_RES := 1080
TARGET_INCLUDE_STOCK_ARCORE := true

# GApps
TARGET_GAPPS_ARCH := arm
TARGET_MINIMAL_APPS := true

# Device identifier. This must come after all inclusions
PRODUCT_DEVICE := surnia
PRODUCT_NAME := aosp_surnia
PRODUCT_BRAND := motorola
PRODUCT_MANUFACTURER := motorola

PRODUCT_ENFORCE_RRO_TARGETS := \
    framework-res

PRODUCT_GMS_CLIENTID_BASE := android-motorola

PRODUCT_SYSTEM_PROPERTY_BLACKLIST := ro.product.model

PRODUCT_BUILD_PROP_OVERRIDES += \
    PRODUCT_NAME="Moto E LTE"

$(call inherit-product-if-exists, vendor/motorola/surnia/surnia-vendor.mk)
