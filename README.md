# lkm-hidden

A Linux kernel module which hides itself.

## Usage

Build this kernel module:
```shell
make
```

Load `lkm-hidden`:
```shell
sudo insmod hidden.ko
```

Then, you can NOT figure out the kernel module.
```shell
cat /proc/modules | grep hidden
ls -l /sys/module/ | grep hidden
``` 

## License

`lkm-hidden` is released under the MIT license. Use of this source code is governed by
a MIT-style license that can be found in the LICENSE file.
