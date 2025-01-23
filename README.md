# PXL-Clock

Welcome to the **PXL-Clock** repository! This repo serves as a central hub for:

- **Official releases** (firmware, software, etc.)  
- **Issue tracking** and **idea proposals** (hardware, software, use cases, features)  
- **Resources for creating custom PXL-Clock applications**

We’re excited to see what the community will build around the PXL-Clock. Below you’ll find everything you need to get started.

<p align="center">
  <img width="640" alt="image" src="https://github.com/user-attachments/assets/4c898f7e-56ae-4a8b-be34-464ad83a5ffb" />
</p>

---

## Order Your PXL-Clock!

Exciting news: ordering the PXL-Clock will soon be possible! 🎉

We’re currently working on the first 100 units, the MK1 edition! We’re in the certification and refining all the little details that make this a fine product. We’re fully committed to delivering something amazing, and we’ll keep you updated every step of the way.

Stay in the loop by following the #pxlclock hashtag on our channels for the latest news and progress updates.

Thank you for your patience and support! 💡

---

## Get In Touch

### Discord

Get in touch with us and others on our [**Discord Server**](https://discord.gg/KDbVdKQh5j)

<p align="center">
  <h3>Join the PXL-Clock Community on Discord</h3>
  <a href="https://discord.gg/KDbVdKQh5j">
    <img src="https://img.shields.io/badge/Discord-Join%20Server-blue?style=flat-square&logo=discord" alt="Join Our Discord">
  </a>
</p>


### Bluesky

Follow the [**#pxlclock hashtag**](https://bsky.app/hashtag/PXLclock) on **Bluesky** for getting news and see what others do!

---

## Table of Contents
1. [Order Your PXL-Clock](#order-your-pxl-clock)
2. [Get In Touch](#get-in-touch)
3. [About PXL-Clock](#about-pxl-clock)  
4. [Releases](#releases)  
5. [Filing Issues and Ideas](#filing-issues-and-ideas)  
6. [Developing Your Own Apps](#developing-your-own-apps)  
7. [Contributing](#contributing)  
8. [License](LICENSE.md)

---

## About PXL-Clock
The **PXL-Clock** is a device designed to display various fun clocks, animations, short stories, visuals and other creative things - all on a 24x24 pixel display. Whether you want to keep track of the current time in a futuristic manner or develop your own mini-apps to run on the clock, this project provides a flexible platform for creativity.

---

## Releases
You’ll find our official firmware and software packages under the [**Releases**](../../releases) section. The PXL-Clock updates itself over-the-air, so no manual steps required.

---

## Filing Issues and Ideas
Have an idea for a new feature or discovered a bug? Help us improve the PXL-Clock by creating a new issue in this repository. We welcome:
- Hardware-related feedback or design modifications
- Software feature requests, improvements, or bug reports
- Use case suggestions or creative ways to integrate PXL-Clock into your projects

Just head over to the [**Issues**](../../issues) tab and click **New Issue** to get started.

---

## Developing Your Own Apps

[![NuGet](https://img.shields.io/nuget/v/Pxl.svg?style=flat-square&logo=nuget)](https://www.nuget.org/packages/Pxl)
[![NuGet Downloads](https://img.shields.io/nuget/dt/Pxl.svg?style=flat-square)](https://www.nuget.org/packages/Pxl)


Whether you’re a seasoned developer or new to programming, we hope these resources will jumpstart your creativity.

You can use this repository as a reference point for developing your own custom PXL-Clock applications. We provide examples, documentation, and tools to help you get started:

To programm PXL-Apps, you need to set up your development environment. Here’s how to get started:

### Prerequisites

**Frameworks**

- [**.NET 8 SDK**](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)
- [**Node / npm** - current LTS](https://nodejs.org)

**Tools**

- [**Visual Studio Code (VSCode)**](https://code.visualstudio.com/)
- [**Ionide-fsharp Extension for VSCode**](https://marketplace.visualstudio.com/items?itemName=Ionide.Ionide-fsharp)

### Fork the Repository

Best practice is to fork this repository to your GitHub account. This way, you can experiment with the code and save your changes, and maybe there will be some surprises along the way. 🎁

### Create Your First App

A PXL-App consists of two parts:

- one or more F# script (or many of them) that contain the code for your app,
- optionally some assets like images.

To set up your first app, simply create a new F# script file in the `./apps` directory. You can use the existing apps as a starting point to learn more about the structure of a PXL-App.

### 🚀 Start the Simulator

Before running any apps, you’ll need to start the simulator.

**Important:** ⚠️ Only one simulator should be running at a time.

1. Open the list of build tasks in VSCode:
   - Press `Ctrl+Shift+B` (Windows/Linux) or `Cmd+Shift+B` (macOS).
2. Select **Start Simulator** from the list.

As an alternative for the VSCode build task, just run `./start-simulator.sh` (Mac) or `./start-simulator.ps1` (Windows) in your terminal.

### Run an App

- Ensure the simulator is running (see above).
- Open your app file in the editor (works as well with all samples and tutorials here in this repo).
- Select the entire content of the file and run it by pressing `Alt+Enter` (Windows) or `Cmd+Enter` (Mac).

You can modify the code, open new files, and re-run apps as often as you like. Simply re-evaluate the **entire file** (that's the mose easy way.)

In case the simulator does not what you expect (e.g. you were in sleep mode), just restart the simulator.

### Submit Your App

When you’re ready to submit your app, create a pull request (PR) with your changes. We’ll review your app, provide feedback or merge it.

Follow-up PRs (updates) for your app in case you want to improve it are welcome!

### The PizzaMampf Sprite

Check out the sprite 🖼️ `./apps/03_ Demos/assets/pizzaMampf.png`) and swap them with your own custom artwork to personalize your app.

### Deploying an App or an Image to the PXL-Clock

Here are 2 ways of deploying an app or an image to the PXL-Clock. Keep in mind that
- the PXL-Clock needs to be connected to the same network as your computer.
- the artifacts you deploy are not persistent (for now) and will be lost after a reboot.

There are two ways to deploy an app or an image to the PXL-Clock:

**Using the VSCode Build Tasks**

Open the list of build tasks in VSCode:
- Press `Ctrl+Shift+B` (Windows/Linux) or `Cmd+Shift+B` (macOS).
- Select **Deploy App** or **Deploy Image** from the list.

**Using the Scripts Directly**

In your terminal, run the following scripts:
- `./deploy-app.sh` (Mac) or `./deploy-app.ps1` (Windows) to deploy an app.
- `./deploy-image.sh` (Mac) or `./deploy-image.ps1` (Windows) to deploy an image.

---

## Contributing

Contributions from the community are highly encouraged. If you want to help make PXL-Clock better, you can:
1. **Create an Issue:** File a new issue for suggestions, bug reports, or feature requests.  
2. **Submit a Pull Request:** Fork this repo, make your changes, and submit a pull request. Make sure to include a clear description of what you’ve changed or fixed.  

Before contributing, please review our [**Code of Conduct**](CODE_OF_CONDUCT.md) (if available) to ensure a positive experience for everyone.

---

see: [LICENSE.md](LICENSE.md)

---

Thank you for your interest in the PXL-Clock! We look forward to seeing your ideas and contributions. If you have any questions or suggestions, feel free to open an issue or start a discussion. Let’s make time more fun—together!
