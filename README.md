# crops_poky

***20211022 - This workaround is no longer needed, the images have been rebuilt by crops***

Update crops/poky:ubuntu-* images to add new ssl certs to fix letsencrypt ssl issue

https://github.com/crops/poky-container/issues/68

https://github.com/jcormier/crops_poky/pkgs/container/crops_poky

Testing:

```
docker run ghcr.io/jcormier/crops_poky:ubuntu-18.04 git clone https://git.linaro.org/toolchain/gcc.git
Status: Downloaded newer image for ghcr.io/jcormier/crops_poky:18.04
Cloning into 'gcc'...
```

```
docker run ghcr.io/jcormier/crops_poky:ubuntu-20.04 git clone https://git.linaro.org/toolchain/gcc.git
Status: Downloaded newer image for ghcr.io/jcormier/crops_poky:18.04
Cloning into 'gcc'...
```
