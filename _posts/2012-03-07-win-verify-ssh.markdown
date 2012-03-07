---
layout: default
title: Verify Your SSH Keys
description: A quick guide to help you verify your SSH keys using the fingerprint
---

<p class="intro">
  This is the guide to verifying your SSH keys in <strong>Windows</strong>.
  There are also guides for <strong><a href="/mac-verify-ssh">OS X</a></strong>
  and <strong><a href="/linux-verify-ssh">Linux</a></strong>.
</p>

<p>
  GitHub uses SSH keys to establish a secure connection between your computer
  and GitHub.
</p>

<p>
  To verify your SSH keys you need to find the <b>fingerprint</b> of each key
  on your computer and compare it to the fingerprint displayed on GitHub.
</p>

<p>
  If there are keys on your GitHub account that you don't recognize you should
  <b>delete them immediately</b>.
</p>

## First: What's a Fingerprint?

An SSH key's fingerprint is a sequence of bytes unique to that key. Fingerprints
are usually encoded into hexadecimal strings and formatted into groups of
characters for readability.

We display SSH key fingerprints on GitHub along with the key's title:

![](https://img.skitch.com/20120307-gy4e74ah5yftbddhmjnsypatnr.png)

## Next: Find and Compare Fingerprints

There are several programs that can be used for getting the fingerprint of an SSH key.

GitHub provides one program, <strong>GHKeyBrowser</strong>, which can be downloaded from
<a href="https://s3.amazonaws.com/github-assets/GHKeyBrowser.exe">https://s3.amazonaws.com/github-assets/GHKeyBrowser.exe</a>

The program will list all your ssh keys with fingerprints.

![](https://img.skitch.com/20120307-gkb7f2bb9ui1r6s9un8jq8k4iy.png)

Another program is <strong>PuTTYgen</strong>, which can be downloaded from 
<a href="http://the.earth.li/~sgtatham/putty/latest/x86/puttygen.exe">http://the.earth.li/~sgtatham/putty/latest/x86/puttygen.exe</a>

Just load the local key file (containing the secret key) into the program and you will see the fingerprint in the textbox labeled "Key fingerprint".


Now open <https://github.com/settings/ssh> and make sure the fingerprints attached to
your GitHub account match the fingerprints in <strong>GHKeyBrowser</strong> (or <strong>PuTTYgen</strong>).

![](https://img.skitch.com/20120307-du7pgft9s9nbm4gwm8isyp7gwr.png)

If the fingerprints match, mark the key as verified.

## Fingerprints don't match?

If there are any SSH keys attached to your account that you don't recognize
<b>delete them immediately</b>.

If all the fingerprints match then you are safe - continue social coding.
