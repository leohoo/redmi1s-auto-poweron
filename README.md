# redmi1s-auto-poweron

## unpack boot.img

https://github.com/HappyZ/dpt-tools/wiki/boot.img-unpack-and-pack

## edit init.rc

https://forum.xda-developers.com/android/general/tutorial-modify-boot-img-to-power-phone-t3456325

change 
```
on charger
    class_start charger
```

to 
```
on charger
    setprop sys.powerctl reboot
```

## about cpio
cpio on mac not working, unpack & repack ramdisk on centos.
