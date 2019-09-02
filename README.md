# solve-lg-gram-17-linux-boot-error
Solve! LG gram 17 linux boot infinite acpi error for kernel 4.18 over

I found a workaround for apci infinite error in LG Gram 17 inch kernel 4.18 and above. I just tested it and successfully booted ubuntu 19.04 kernel 5.0.

In the meantime, many Linux in the world have been uncomfortable with this problem. It seems to be able to help enough, but stick to the policy that the OS can not help any other than Windows, so I'm disappointed with the manufacturer LG, who didn't give any help.

I  looked at all the settings for the 14-inch grams of 2018 that were before 17 inches and found the differences to find the cause. The workaround is as follows:

1. At boot time, press F2 to enter bios.
2. Press ctrl + alt + F7 to switch to advanced mode.
3. Select the advanced tab.
4. Select Intel Advanced Menu.
5. Select Thunderbolt (TM) Configuration.
6. Select Discrete Thunderbolt (TM) Configuration.
7. Select Thunderbolt (TM) OS Select.
8. Set Windows 10 Thunderbolt support to Disabled. After a delay of about 5 seconds after setting, the confirmation message for saving the setting changes appears.
9. Save the changed settings and reboot.
10. Now you can boot normally with the latest kernel! enjoy linux!


I got a hint and the link is https://github.com/dhedlund/kernel-patch-lg-gram-17 and I found that it seems to be a problem with Thunderbolt.

Thank you.
