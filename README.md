# MacBookAir61_ubuntu_wifi
wifi drivers for MacBookAir6,1 on ubuntu 16.10

Install dkms

`$ sudo dpkg -i '/path/to/dkms_2.2.0.3-2ubuntu14_all.deb'`

Install bcmwl-kernel-source

`$ su_i kg -i  '/path/to/bcmwl-kernel-source_6.30.223.248+bdcom-0ubuntu8_amd64.deb'`

Make it so

`$ sudo apt-get install -f `

# Now fix the problem of the display shutting off from resume

`$ sudo dpkg -i '/path/to/mba6xbl-dkms_1.0.0_all.deb' `
`$ sudo modprobe mba6x_bl`
`$ gnome-session-quit`

