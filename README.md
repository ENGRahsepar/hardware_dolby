™ë,j¢Ñhºw]¡Ë¦z{Z¶*'º¹a¶Úlÿ÷hrÈ"¶›r‰¿­ë-ş·©¢ÏÜ¢{^Û zÚŞ¦‹"¶Šòr‰íz{lµ«n³8
Infinity X (xaga) note
----------------------
In the Infinity X 4.1 xaga build, `vendor.dolby.media.c2@1.0-service` is dropped
from packaging (dolby.mk): the vendor c2 HAL crashes on Android 17 (vendor
RefBase ABI mismatch) and takes mediaserver down mid-session. The Dolby audio
effect side (dms service) remains shipped and enabled. Gate that c2 service out
of your device tree on A17 rather than fighting the crash.
