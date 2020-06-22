# @ataberkylmz/hx711

This is a fork of [**@shroudedcode**'s `hx711` package](https://github.com/shroudedcode/hx711) which is also forked from [**@dangrie**'s `hx711` package](https://github.com/dangrie158/hx711).

I've modified the library in such a way that it does not use 100% of the CPU all the time. Currently the usage is about 15-20% on Raspberry Pi 3 B+. This CPU usage is also reducible if we can figure out the sensor's response time and sleep till we possibly have a valid response. Currently the default sleep time is set to 100 nanoseconds.

This version also uses **Broadcom GPIO pin numbering**  instead of physical/board numbering.