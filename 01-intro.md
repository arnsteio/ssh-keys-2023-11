---
title: BASH novice
teaching: 150
exercises: 0
objectives:
- "Understand why learing the UNIX shell is a good idea"
- "Automating repetitive tasks"
- "Documenting data maniplulation steps for reproducible reseach"
---
# Introduction to the UNIX shell

1. [This lesson](#this-lesson)
2. [Why learn to use the shell?](#why-learn-to.use-the-shell)
3. [Copying the key to VGL](#copying-the-key-to-vgl)
4. [Important files](#important-files)

## This lesson

I will spend somwhat more than two hours on the UNIX shell, basing my teaching on the Software Carpentry [Shell Novice](https://swcarpentry.github.io/shell-novice/) lesson. 
Ii is unlikely we will get to the end of the lesson, but you may follow though to the end in your own time.
If you are already familiar with the shell you may wish to go to the [Shell Extras](https://carpentries-incubator.github.io/shell-extras/) lesson instead, and follow that through self-study. 

At 11:15 I will go through SSH keys and we will all generate an SSH key pair and make sure our public key is uploaded to the PPI machines. 
This key will also be useful for the Gitlab lesson following this lesson. 

## Shell nowice
- [Shell Novice](https://swcarpentry.github.io/shell-novice/)
alternatively, in your own time,
- [Shell Extras](https://carpentries-incubator.github.io/shell-extras/) 


### SSH keys
[SSH keys](https://arnsteio.github.io/ssh-keys-2023-11/)

## Important files

Your ~/.ssh catalog has your key pair. 

- id_rsa is your private key. *keep it secret, keep it safe!*
- id_rsa.pub is your public key 

On a server,

- authorized_keys has a copy of your public key


> Excercise: Can you find out how many SSH keys you have at the PPI system?
>
>> Solution: 
>>~~~
>>ssh ppi-r8login-a1.int.met.no
>>cat .ssh/authorized_keys | wc -l
>>~~~

> Excercise: If you have more SSH keys than you need, shall we clean the excess ones out?
>
>> Solution:                               
>>Log in on the PPI system and remove unnecessary files from the ~/.ssh/authorized_keys file. 
>>We have worked a lot with things like this today!


[Previous slide](README.md)
[Next slide](02-End.md)
