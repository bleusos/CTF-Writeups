#helithumper_re

Download binary: https://github.com/guyinatuxedo/nightmare/blob/master/modules/03-beginner_re/helithumper_re/rev

![alt text](/photos/image.png)

At first glance, the program is checking for a specific pass phrase.
In Ghidra, we can see that there is a function call "validate" in the main function.

![alt text](/photos/image-1.png)

If we inspect further, it seems like this validate function is checking pre-set hex values.

![alt text](/photos/image-2.png)

Let's plug these hex values into CyberChef and see if we get anything useful.
![alt text](/photos/image-3.png)

Boom. The flag: flag{HuCf_lAb}
Let's verify by inputting it into the binary.

![alt text](/photos/image-4.png)
Success.
