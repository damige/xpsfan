# xpsfan

-- WARNING, your laptop may overheat! use with caution. I will not be responcible for any damages --

Arch-linux Tool to lock the fan on dell XPS13 (9350)

Run xps_fan-unlock / xps_fan-lock / xps_fan-silent  / xps_fan-original with root

xps_fan-silent will disable turbo mode, lock cpu to 1ghz, intel gpu to minimum (300mhz for iris 540) and lock the fan for silent running.
Go into silent mode when the fan is already off, as it will lock the fan in that state.
Silent mode requires intel driver (not modeset) as it lowers gpu speed through intel supplied tools

xps_fan-original will reenable turbo, allow cpu to max (3.2ghz i7 6560U) and intel gpu up to max (1050mhz for iris 540)

On testing my laptop will run up to 95c after a few minutes of stresstesting (gaming) running on 1.2ghz makes it 100c and throtting seems to occur.
Using a 4 thread cpu stresstest temps are ~65c
Normal usage for me temps and performance is fine. (browsing, coding, etc)
GPU seems to be the main contributor to the heat, if not using the gpu intensively i have found that the cpu frequency can be set higher (tested ~1.6ghz).

TODO:

- more testing
- ??

-- WARNING, your laptop may overheat! use with caution. I will not be responcible for any damages --

