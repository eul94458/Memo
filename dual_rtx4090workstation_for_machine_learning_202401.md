# Dual RTX4090 GPU Workstation for Machine Learning (2024/01)

## Parts

This is a 2 * RTX4090 shopping list because we are poor.

### GPU

(unit: slot = ~20mm)

For RTX4090, you are looking at 4 slot/each GPU.

Go for as many 3 slot RTX4090 as possible otherwise you are limited to the choice of case and motherboard.

Also, you don't want any liquid leakage happening, thus only air cooled GPU are considered here.

The followings are more or less 3 slot:

- PNY RTX4090 Vetro LED
- Gigabyte RTX4090 Windforce V2
- MSI RTX4090 Gaming X Slim

### PSU

RTX4090 rated at 450W but rarely go beyond 300W in real world machine learning task, as far as in my use case. So 2 * RTX4090 you are looking at 2 * 450W (GPU) + 300W (GPU) = 1200W. You can go for 1500W for larger headroom to enhance expandability (so that 3 * RTX4090 or more advanced future GPU setup is available) and stability (high power usage spike of one RTX4090 can go beyond 300W).

Make sure you are buying ATX3.0 standard PSU. Old standard will do but this new standard is better.

### Case

You must buy a case with bottom intake fan to not choke your GPUs.

For 3 slot RTX4090, pick a big ass case with at least 8 expansion slot. Some cases will have plenty of room at the bottom for thicker water cooling radiator, despite listed as 7 slot, that extra room can account for 1 more slot space.

- Fractal Torrent
- Thermaltake Core P8

For 4 slot RTX4090, pick a big ass case with at least 9 expansion slot.

- Fractal Define 7 XL
- Fractal Meshify 2 XL
- Thermaltake View 51
- Lian Li O11 Dynamic XL
- Lian Li O11 Dynamic Evo XL

Or any mining rig will do.

### Motherboard

The choice of CPU is limited by the fact that not all motherboard suport dual GPU configuration i.e. x8/x8 bifurcation, and not all x8/x8 motherboard has enough space between the two PCIe slot to fit 4 slot GPU.

For 3 slot RTX4090 (if you don't mind choking the upper GPU):

- Asus Z790 ProArt Creator (7 Expansion Slot)
- Asus ROG Maximus Z790 Hero (7 Expansion Slot)
- Asrock Z790 Taichi (7 Expansion Slot)
- Asrock Z790 Taichi Carrara (7 Expansion Slot)
- Asus X670E ProArt Creator (7 Expansion Slot)
- Asrock X670E Taichi (7 Expansion Slot)
- Asrock X670E Taichi Carrara (7 Expansion Slot)
- EVGA Z790 DARK K (7 Expansion Slot)
- Biostar Z790 VALKYRIE (7 Expansion Slot)

For 4 slot RTX4090:

- Asus ROG Maximus Z790 Formula (9 Expansion Slot)
- Asus ROG Maximus Z790 Dark Hero (9 Expansion Slot)
- Asus ROG Maximus Z790 Apex Encore (10 Expansion Slot)
- Asus ROG Maximus Z790 Extreme (9 Expansion Slot)
- Asus ROG Maximus Z790 Apex (9 Expansion Slot)
- Gigabyte AROUS Z790 Tachyon (9 Expansion Slot)
- Gigabyte AROUS Z790 Tachyon X (9 Expansion Slot)
- EVGA Z790 CLASSIFIED (10 Expansion Slot)
- MSI X670E Crosshair Extreme (9 Expansion Slot)

Of corse you can mix 4 slot (upper slot) and 3 slot (lower slot) to reduce space requirement and this is recommended, otherwise no pc case will fit your big ass lower RTX4090.

Because not all motherboard are build equally, to do CPU or RAM overclocking, I would recommend you to use Gigabyte Z790 Tachyon series. It provide the most stable CPU and RAM power adjustment with one click overclocking (which Asus also claim they can but in reality it always fail). Also if you are considering undervolting you Intel GPU, I have both Gigabyte Z790 Tachyon and Asus ROG Maximus Z790 series in my lab, Gigabyte's can do it more stably than Asus's simultaneously providing more performance.  However, Gigabyte Z790 Tachyon has only 2 RAM slot.

Be careful some highend motherboard only has 2 RAM slot like Arous Z790 Tachyon and Maximus Z790 Apex. Especially if you are aiming at using higher transfer rate and low latency RAM, in most cases less RAM stick on the motherboard means more stability to the system. The memory controller cannot handle too many RAM sticks. For example, DDR5 6400MHz will never be stable at the time I am writing this memo, unless you are memory overclocking mastermind, you basically cannot put in 4 highend DDR5 RAM into the mortherboard and hope that it can run at full speed.

If you need mor RAM capicity, per the forementioned instability issue, you have no choice but choose slower DDR5 RAM so that you can put 4 of them into the motherboard and get 128GB or 192GB.

As Intel Gen 12/13/14 CPU support both DDR4 ad DDR5, some motherboard mentioned earlier may have DDR4 variant. But if you are doing memory intensive work which exactly is machine learning, you must abandon DDR4 to juice more performance out of the configuration.

AMD AM5 architecture support only DDR5 so you left with no choice.

Those motherboard listed above are all highend stuff otherwise lack connectivity or expandability or don't even support 2 GPU configuration. Some series may have mid or low end derivation like Z790 chipset -> B760 chipset or something like that. Those have less feature compared to the their highend counterpart so be careful not buying the wrong one.

### RAM

For the sake of stability, I would recommend you to buy those RAM that has enough high transfer rate natively. For DDR4, you should find one that is rated at 1.2V. For DDR5, find 1.1V. However, running at high transfer rate natively doesn't mean that you can escape from the 4 stick DDR5 curse. Still they are running at a high transfer rate and the memory controler cannot handle 4 of them, the BIOS will make them all run slower together, like 4800MHz.

### CPU

Depends on what motherboard you have, pick the appropriate CPU brand. Go for a better CPU so that your GPU thought-put and RAM speed will not bottlenecked by the CPU.

Z790 chipset -> Intel Gen 12/13/14

X670 chipset -> AMD AM5 of whatever generation it is

### CPU Braket

If you choose Intel CPU i.e. LGA1700 socket, buy 3rd party CPU braket to better sit the CPU flat. This can reduce 5 up to 10 degree celcius under load. But do it carefully. Do not shake your hand or drop anything onto the CPU socket otherwise pins bend and then the motherboard become useless.

### CPU cooler

Make sure the height of CPU cooler can fit inside your PC case. Never buy server grade CPU cooler because they are lousy and sucked.

### SSD

Consult reviews to see the performance.

Avoide the brand Crucial at all cost since they are absolute e-waste in terms of sustained write performance. Even HDD is faster than that. Otherwise, WD, Samsung, Seagate, they are good to go. SK Hynix is also top tier performance but some independent report said they are prone to data loss during power-loss, so you think about it.

It would be better if you can get enterprise grade SSD, they max-outed on durability. But be careful that they might use plug other than M.2, for instance **U.2**, hence motherboards listed above are not compatible at all. You might need server grade motherboard and CPU for that.

## Troubleshoot

### Nothing shown on screen after POST

Make sure you connected HDMI/DP/TypeC cable into the monitor and GPU.

If your CPU don't equipped with iGPU, plug the cable into discrete GPU. Try different HDMI/DP/TypeC slot to see if this is the problem of defected output socket.

If already plugged into the correct HDMI/DP/TypeC slot, try to pull and replug the cable so that the motherboard re-detect the monitor, usually the screen will then work again.

If none of the above is doing anything, clean the CMOS of the motherboard. Every motherboard brand has their own way to do this. You must consult the **user manual** before doing so to prevent hazard. After cleaning CMOS, retry all the above strategies.

If still nothing being shown on screen, try shut down the computer and unplug the power cable. If you are dealing with discrete GPU, re-sit the GPU. What means by re-sit, it means pull it out and put it back again into the same slot. Still nothing? Try different slot.

If not, try a different GPU to see if the problem is the GPU. Or try a different RAM to see if the problem is at the RAM.

If problem still consist, try re-sit the CPU and CPU cooler. Maybe you applied the screws too tight making some motherboard pins not touching the CPU. On the same line, check if any bended CPU pins on either the motherboard side or CPU side.

If the issue consistent, consider that anything one of more thing is broken at the first place.

## Set Up

### Enter BIOS

Usually you can access the BIOS menu by spamming **Del** key on the keyboard. Some manufacture use **Esc** or **F10**. You may try all of them if you don't know which it is.

### Confirm Hardware Info

BIOS will list up information about the hardware. Make sure it displaying correct CPU, RAM, RAM capacity, RAM speed, GPU, etc. Some manufacturer might not have GPU info shown on their BIOS menu.

For some motherboard, the very first boot up might not display the correct RAM speed. But the second boot will be fine.

### RAM Overclock

If you installed high-end RAM which can auto overclock through XMP or something, make sure you are enabling XMP option in the BIOS to let the RAM run at its optimal speed.

### Fan Speed

Since you have 2 * RTX4090 inside the case, you need more air flow than usual. There should be fan settings in modern BIOS menu, find it, and set CPU fan curve to normal and case fan more than normal (like turbo or something, exact wording depends on the manufacturer).

### Resize Bar

You must enable this feature for better GPU performance.

### Bifurcation

You must set x8/x8 bifurcation since you are using two GPU. Some motherboard got their PCIe lane share the same bandwidth with the fastest M.2 slot, you can have either 1GPU+1M.2 or 2GPU configuration. Abandon the fastest M.2 slot for the sake of our GPU.

### CPU Undervolt

CPU manufacturers push their CPU to the limit out of box and it is hot as shit. By undervolting it, which means set the CPU to run in 0.1 less volt, it can keep the same performance while running 10 degree Celcius cooler than before. However, depends on the power module of your motherboard, it might not be stable at -0.1Volt, if so, try -0.05Volt.

### System Stability

How do I know if my system is stable? Boot into Windows, launch Cinebench and run benchmark for 10mins. If Cinebench or the OS do not crash, I think you can consider your system as stable. Otherwise, like setting -0.1 volt for CPU in ASUS motherboard, Cinebench cannot run second iteration on CPU benchmarking, it will stop and unresponsive for no reason.

### GPU ECC

RTX4090 has ECC on it. If you are academia, you should enable it.  

### PCIe lane sharing

As mentioned before, some motherboard split the fastest PCIe lanes to PCIex16 slot and M.2 slot. So you can use either 2GPU+0SSD, or 1GPU+1SSD. Make sure you are not putting the SSD into that shared M.2 slot. Consult the user manuel for details.

### iGPU priority

If your GPU has iGPU inside, you can off load displaying work to it and release all discrete GPU's power to computing. However, installing Linux will fail under this circumstances. You may disable using iGPU by enabling CSM compatibility in the BIOS menu. Disable the iGPU for the moment to install Linux, after you have your Linux installed in your SSD, you can re-enable the iGPU again.

### RAID

Heard that RAID may harm SSD durability but I don't know. Research yourself.


## Installing Linux

### Out of memory. Error message shown that it is related to graphics.

If the CPU has iGPU in it, it can be fixed. Reboot and enter BIOS menu. Enable CSM mode to disable iGPU, save settings and reboot. But make sure you have a discrete GPU so that you can see stuff. After disabling iGPU, re-enter Linux install media, you should be fine.

### No Wifi

God bless you if you have a Wifi USB stick hanging around. The issue is due to lack of wireless driver for the motherboard. Your Wifi USB stick should enble you to connect to the Internet. And then, you go to the update center to update stuff. Hope your motherboard manufacture publish the appropriate driver to the repository. Reboot after updating. After that you should be fine but mostly Linux update are never gonna be fine. You got infinite amount of new bug but hey, at least the Wifi chipset is working! (or is it?)

### ptxas version not match

The machine learning framework JAX rely on CUDA. Sometime CUDA library is not properly installed or installed with a wrong version. And the runtime error message may show you that **ptxas has problem** something like that. You can fix this by installing cuda stuff (CUDA toolkit) through conda instead of using Linux system's own package manager.

```conda install -c nvidia cuda-nvcc```

The above code will install CUDA compiler and stuff through offical Nvidia channel using Anaconda virtual environment.

### I followed instruction online to install Nvidia CUDA but nuked screen output

Some folk may told you to purge *nvidia and reinstall the GPU driver, and then stuff happens. I did this before and I knew how it feels. I figured out the reason is that that default motherboard driver (I guess) which is Xorg stuff also got nuked simultaneously following Nvidia stuffs. By that, you lost Internet access through neither Wifi nor Ethernet cable thus you can't ```apt-get install``` stuff. Well, grap a USB drive and download the Xorg driver also new Nvidia driver by another computer, transfer them to the dead computer, install them and I was able to get my screen back.

But because of the god damn dependency model of Linux, you don't know what else besides Xorg also got nuked during the process. I traced the dependency tree by like 2 levels and installed them back on, Xorg is one of them, it worked, for me.














