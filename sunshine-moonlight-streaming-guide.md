---
title: "The Ultimate Guide to Low-Latency Game Streaming: Sunshine + Moonlight"
excerpt: "Learn how to turn your PC into a personal cloud gaming server. This guide covers setting up Sunshine and Moonlight for high-performance, low-latency gaming on any device."
date: "2026-05-02"
author: "Brandez Tech"
tags: ["Gaming", "Streaming", "Tutorial"]
coverImage: "https://images.unsplash.com/photo-1542751371-adc38448a05e?q=80&w=2000&auto=format&fit=crop"
---

# Turn Your PC into a Personal Cloud Gaming Server

Gaming on a high-end PC is great, but sometimes you just want to sit on the couch and play on the big screen. While solutions like Steam Link or Chromecast exist, they often suffer from noticeable lag and compression artifacts.

Enter **Sunshine** and **Moonlight**—the gold standard for low-latency game streaming.

## Why Sunshine and Moonlight?

Originally, NVIDIA had a feature called "GameStream," but they eventually discontinued it. **Sunshine** is an open-source replacement for the host side (your PC), and **Moonlight** is the client app that runs on your TV, phone, or tablet. Together, they offer:

*   **Near-Zero Latency:** Superior to almost every other streaming solution.
*   **High Quality:** Supports 4K resolution, HDR, and up to 120 FPS.
*   **Multi-Platform:** Works on Android TV, Apple TV, iOS, Linux, and more.

## Video Tutorial

If you prefer a visual guide, check out our full setup walkthrough here:

[![Watch the Setup Guide](https://img.youtube.com/vi/O68MS9dXOPw/0.jpg)](https://www.youtube.com/watch?v=O68MS9dXOPw)

## Step-by-Step Setup

### 1. Install Sunshine (The Host)
Download the latest release from the [Sunshine GitHub repository](https://github.com/LizardByte/Sunshine). 
- Install the application and open the web interface (usually `https://localhost:47990`).
- Create a username and password.
- Ensure your firewall allows the necessary ports.

### 2. Install Moonlight (The Client)
On the device you want to play on (Smart TV, Phone, etc.), download the **Moonlight Game Streaming** app from the respective app store.

### 3. Pairing
- Open Moonlight on your client device. Your PC should appear automatically if you are on the same network.
- Click on your PC. A 4-digit code will appear on the client.
- Go back to your PC, enter that code into the Sunshine web interface under the "PIN" tab.

### 4. Optimize for Performance
- **Ethernet is King:** For 4K streaming, try to have both your PC and your TV connected via Ethernet.
- **Bitrate:** Start with 20-30 Mbps for 1080p and 50+ Mbps for 4K.
- **HEVC (H.265):** Ensure HEVC is enabled in Moonlight settings for better quality at lower bitrates.

## Conclusion

With Sunshine and Moonlight, you no longer have to choose between the power of a PC and the comfort of a console. You can have both. 

Happy gaming!
