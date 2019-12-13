---
title: Why Linux?
category: programming
---

I have been using Linux for a while now (about six months). I started out of need (my laptop was very, very slow, and a friend of mine to give Linux a try, as it was way less bloated than Windows (it's not that hard to be less bloated if Windows is your comparative OS). At this point i was frustrated by the slowness of Windows, so i decided to install Ubuntu.

To be honest, i didn't use Linux as much as i would've liked during this time: i tried basic commands, but i never got that deep into the rabbit hole.

Everything changed when i got a new laptop.

I wanted to delve deeper into the world of Linux. I had read that Linux (and any Unix-based OS) is very good for programming, and i wanted to know why that was. So i decided to install Manjaro on my recently bought Razer Blade, and i was marvelled by the amazing tools the OS gave to me.

So, to answer the title question:

* You know where your stuff is. In Windows, it was usually the case that i had no idea where the wizard i had used to installed a program had left the files in. Even worse, if i found the installation directory of a program, the installation path was not consistent among programs! The `pacman` builtin app manager is really neat, because it manages everything for you and always installs programs into the same directory, all from the command line! If i want to install, say python, i can write

```shell
sudo pacman -S python
```

And that's it! I don't have to download an installer from the official Python page! It as later that i discovered that this wasn't a Linux-exclusive feature, as the same concept exists under the name of Homebrew in MacOS and Chocolatey in Windows. However, the way pacman organizes packages is still very consistent, which is a big advantage for me.

* Customization! It really depends on window manager you choose. For instance, KDE is not very customizable (in fact, i'd say it's almost as static as Windows); XFCE is a bit more customizable. And then there is the world of tiling window managers, which give you a lot of freedom regarding cutomization. I'm currenyly using i3, and i'm loving it so far (for more on the customization topic, refer to [this link]([200~https://www.reddit.com/r/unixporn/). I specifically like the fact that, in most programs that i use, the configurations are nothing more thann a file located in the `/home/.config` folder still amazes me.

* The Unix philosophy. Summarized in a single word: *modularization*. For intance, my text editor (which every day feels more like an IDE) comes with nothing but a few features (syntax highlighting, very useful keybindings, and what have you), and i have been adding plugins on demmand. There's not a single plugin i don't use. The fact that i have become very familiar with my development environment makes me feel confident when working, as i know what each thing does, and i know that if i need anything i can use a plugin for it or write my own.
