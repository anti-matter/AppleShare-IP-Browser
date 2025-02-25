<p align="center">
  <img src="https://github.com/user-attachments/assets/2385267d-73f2-4b37-8898-e744b0f9276c"/>
</p>

# AppleShare IP Browser

## Introduction

Let me get started by saying that I wrote this application because it filled a need I have, which is to quickly and reliably access files on a central server from Macs that I'm restoring (see Figure 1 as an example). Due to server reliability and availability, I run an AppleShare IP server on either my Windows or Haiku OS machines (mostly my Haiku machine). So, while servers on these system can be accessed from OS 8.0 and later with no issue, gaining access to them from older OS's can be challenging, particularly where OpenTransport is not desired, or an option.

<p align="center">
  <img style="width: 50%; height=50%" src="https://github.com/user-attachments/assets/f89b5dbd-e74b-4ed6-8e4a-9a84d559c856"/>
</p>

What sort of worked was installing OpenTransport (with System 7.1 or later) and then copying over the AppleShare client that came with MacOS 8.0, AppleShare Client 3.7.1. Using another version on a 68K mac would crash the machine as soon as you mount an AppleShare IP volume.

So, I began writing my own AppleShare IP client so I could access shares not only on my MacOS 9 macs, but also on my Haiku and Windows machines. And, so it works on the older macs, support for MacTCP was a must since 68000 machines don't support OpenTransport.

To checkout my AppleShare IP Server for Haiku or Windows, just visit the following links to download and use them for free (some day I will get the naming straight between the two).
- https://github.com/anti-matter/MacFile_For_HaikuOS
- https://github.com/anti-matter/Windows_AFP_Server

## System Requirements

To run the AppleShare IP Browser, you need:
    - System 7.0 or later
    - MacTCP or OpenTransport installed and configured
    - A 680x0 or PowerPC Macintosh
    - At least 2mb of free RAM

If you end up low on RAM while transfering a large number of files, try increasing the RAM allocated to the application so it has more room to build the transfer tables.

## Connecting
To simplify connecting to a server a bit, I combined entering the IP address of the server you're connecting to and entering your credentials into a single window (Figure 2).

<p align="center">
  <img style="width: 50%; height=50%" src="https://github.com/user-attachments/assets/5fb82a71-eed7-48be-94ed-b06ca670609f"/>
</p>

## Browsing
Browsing is accomplished by choosing a volume from the volume list, then navigating in the lower list down through the files and folders on the share. Items in bold are folders and when double-clicked, you will traverse into the folder's contents.

<p align="center">
  <img style="width: 50%; height=50%" src="https://github.com/user-attachments/assets/f9693979-e6d0-47c9-a6b8-ef8a7958791f"/>
</p>
