# Ganglion Getting Started Guide
###Overview

This guide will walk you through setting up your Ganglion, connecting it to your computer, and then connecting it to yourself. The first tutorial is for Mac users, the second is for Windows users. Please review this guide in its entirity before starting. Have fun! 

**Note that the Ganglion is not set to be discoberable out of the box, you need the GUI or another app. 

## What You Need

![OpenBCI Contents](../assets/images/ganglion_what_you_need.png)

 1. OpenBCI Ganglion Board
 3. 6V AA battery pack & (x4) AA batteries (batteries not included)
 4. (x4) plastic feet for board stabilization
 5. OpenBCI [Gold Cup Electrodes](http://shop.openbci.com/collections/frontpage/products/openbci-gold-cup-electrodes?variant=9056028163), or your own electrodes, and [Electrode Paste](http://shop.openbci.com/collections/frontpage/products/ten20-conductive-paste-2oz-jars)
 6. [Snap Electrode Cables](http://shop.openbci.com/collections/frontpage/products/emg-ecg-snap-electrode-cables?variant=32372786958) and [Snap Electrodes](http://shop.openbci.com/collections/frontpage/products/skintact-f301-pediatric-foam-solid-gel-electrodes-30-pack?variant=29467659395)
 7. A computer connected to the internet

### 1. Your Ganglion

![OpenBCI 8-bit Top](../assets/images/ganglion_head_shot.jpg)

The battery connector on the back can accept 3V to 12V DC power input. The pushbutton is a reset button. For more information on the Ganglion Hardware, visit the [OpenBCI Ganglion](http://docs.openbci.com/Hardware/07-Ganglion) page in the Hardware section.


### 2. Gold Cup Electrodes and Paste

![Electrode Starter Kit](../assets/images/electrodeStarterKit.png)

If you ordered OpenBCI [Gold Cup Electrodes](http://shop.openbci.com/collections/frontpage/products/openbci-gold-cup-electrodes?variant=9056028163) and [Electrode Paste](http://shop.openbci.com/collections/frontpage/products/ten20-conductive-paste-2oz-jars), it should come with:

 * 10 passive, gold cup electrodes on a color-coded ribbon cable
 * 3 2oz Jars of Ten20 conductive electrode paste

![TouchProof Adapter](../assets/images/touch_proof.jpg)

If you plan to work with your own electrodes, the [Touch-Proof Adapter](http://shop.openbci.com/collections/frontpage/products/touch-proof-electrode-cable-adapter?variant=31007211715) will come in handy. It will convert any electrode that terminates in the industry-standard touch-proof design to an electrode that can be plugged into any OpenBCI Board!

### 4. (x4) Plastic Feet

![Plastic Feet](../assets/images/ganglion_wPlasticFeet.png)

Your OpenBCI kit comes with 4 plastic feet that can be snapped into the holes of your board to provide extra stability while working.

### 5. Your 6V AA Battery Pack & 4 AA Batteries

![Battery Connection](../assets/images/ganglion_batteryConnection.png)

Install 4 AA batteries in your battery pack, plug in your Ganglion board and turn on the power switch. You should see the BLUE LED blink gently. Blinking means that the BLE radio is not connected or paired with any computer or phone/tablet. Once the Gagnlion is connected, the LED stays steady on.

## Download/Run the OpenBCI GUI on macOS

![Bluetooth On!](../assets/images/ganglion_BLE-ON.png)  

First, turn on your computer's Bluetooth.  

Do not use a dongle with macOS. Dongles such as the `CSR` dongle are only needed for Windows and sometimes linux!

![GUI unzip](../assets/images/ganglion_GUI-unzip.png)

Then go to the [GUI Downloads page](http://openbci.com/donation) and download the latest software release for Mac. The GUI is built on [Processing](https://processing.org/), a creative coding language, so you can also download the OpenBCI Processing Sketch and run it through processing. Once you unzip/extract the download, open the file called `OpenBCI_GUI_200_MACOSX` and there you will find the `OpenBCI_GUI.app`. You can move that into your `Applications` folder.  

**NOTE: If you are using a Mac with macOS Sierra, you MUST move the OpenBCI_GUI.app into your Applications folder. You also need to change your Security & Privacy settings to allow apps from Anywhere. Go to the [end](http://docs.openbci.com/Tutorials/02-Ganglion_Getting%20Started_Guide#ganglion-getting-started-guide-run-the-gui-on-macos-sierra) of this page for instructions on how to do that, then come back to conintue this tutorial.**

![allow GUI to run](../assets/images/ganglion_permissions.png)

When you first run the GUI on your Mac, you will have to give administrator permission. You may see a message pop up asking you if you're sure you want to open it. Click `Open` and the app will launch.

![Allow Form Anywhere](../assets/images/ganglion_SysPrefs-Allow.png)

If you have any other trouble with your permissions, or if you don't see the option to `Open` the app, check your `Settings/Security & Privacy` and make sure you tick the `Anywhere` button.

## Download/Run the OpenBCI GUI on Windows

**We are in the process of updating this guide to include Windows 7 users. it *is* possible to use the Ganglion and CSR 4.0 BLE Dongle on Windows 7. For now, please visit this [forum post](http://openbci.com/forum/index.php?p=/discussion/918/ganglion-and-windows-7), which outlines the proceedure.**

![CSR Dongle to USB port](../assets/images/ganglion_win_1_plugCSRDongleIn.JPG)

The OpenBCI Ganglion uses Bluetooth LE (aka Bluetooth Smart, Bluetooth 4.0) and in order to use the Ganglion with Windows, you need a small USB Dongle. We have verified CSR 4.0 Dongles in our [store](http://shop.openbci.com/products/csr-4-0-bluetooth-dongle), and you can get them from various onine vendors.  
**IMPORTANT:** The BLE Dongle *must* be a veriied CSR 4.0 Dongle!  

First plug in your CSR 4.0 BLE Dongle.   

![Searching Zadig in Google](../assets/images/ganglion_win_2_searchZadigInGoogle.PNG)

Then, go to the [Zadig tool website](http://zadig.akeo.ie) to get the driver.

![Windows Vist or Later](../assets/images/ganglion_win_3_downloadZadigForWindowsVistaOrLater.PNG)

Download Zadig for Windows Vista or Later

![Open Zadig Installer](../assets/images/ganglion_win_4_openZadigExe.PNG)

Open the Zadig tool once it's done downloading. Acknowledge the message to allow the program to make changes to your OS.

![No to updates](../assets/images/ganglion_win_5_noToUpdates.PNG)

Select *No To Updates* when prompted.

![Select Options](../assets/images/ganglion_win_6_selectOptions.PNG)

On the top bar select *Options*.

![List all devices](../assets/images/ganglion_win_7_selectListAllDevices.PNG)

Then select *List All Devices*.

![Select CSR](../assets/images/ganglion_win_8_selectCSRFromDropDown.PNG)

Select CSR from the dropdown.

![Replace Driver](../assets/images/ganglion_win_9_selectReplaceDriver.PNG)

Then press *Replace Driver*.

![Driver Installed Success](../assets/images/ganglion_win_10_driverInstalledMessage.PNG)

You should then see a progress bar followed by a success message.

![Driver Installed Success](../assets/images/ganglion_win_11_bothSayWinUSB.PNG)

Note that both drop-downs both say *WinUSB*.  
Great! You are now ready to download the OpenBCI GUI and use your Ganglion!
Go to our [Downloads Page](http://openbci.com/donation) and download the application that suits your Operating System.

## Start Using The OpenBCI GUI

![Live From Ganglion](../assets/images/ganglion_select_LIVE-from-ganglion.png)

Once the GUI is running, select `LIVE (from Ganglion)`. That button will turn green, and you will see a pane open titled `BLE DEVICES`, and a list of Ganglions in the neighborhood. Each Ganglion has it's own unique 4 character ID (in HEX), and you will see it listed in the `BLE DEVICES` window. If you don't see any Ganglions, check to make sure your Ganglion has a battery connected, is switched on, and the blue LED is blinking. If there are multiple Ganglions in the room, you can find yours by turning it off, clicking the `REFRESH LIST` button, then turn on your Gagnlion again. Make a note of *your* Ganglion's 4 character ID.  

![File Name](../assets/images/fileName.png)

**NOTE every time you run the GUI, it will generate a recording to file. You have an option at this point to create your own file name, in the `DATA LOG FILE` window, should you choose to.**  

![START SYSTEM](../assets/images/startSystem.png)

Click on the Ganglion board name that you want to connect to, so that it turns green, and now you are ready to roll! Press the `START SYSTEM` button. It may take up to a minute, but the GUI is setting itself up and connecting to your Ganglion!

![Start Data Stream](../assets/images/ganglion_connected-idle.png)

When the GUI connects, it opens up to the default window layout. For a more indepth guide to the GUI interface and functionality, check out the [OpenBCI GUI](http://docs.openbci.com/OpenBCI%20Software/00-OpenBCISoftware) doc. For the purposes of this introductory tutorial, You should follow the following steps to setup the GUI.  

![select layout](../assets/images/ganglion_select-layout.png)

Click on the `Layout` dropdown menu, and select the one outlined in red.

![Auto Scale](../assets/images/ganglion_autoScale.png)

Click the `Vert Scale` dropdown menu, and change the Veritcal Scale to `Auto`.  

![Accelerometer](../assets/images/ganglion_accelerometer_widget.jpg)
![Accel ON!](../assets/images/ganglion_accel-ON.jpg)

Click the `Head Plot` dropdown menu on the lower right widget container and change it from `Head Plot` to `Accelerometer`. Then turn on the Accelerometer by clicking the `Turn Accel On` button.

![Start Data Stream](../assets/images/ganglion_Start.png)
![First Live Ganglion Data](../assets/images/ganglion_first-data.jpg)  

Now let's get the first data from the Ganglion! Click on the `Start Data Stream` button, and you should see the `Time Series` window scrolling some data to the left, the `FFT Plot` container will show you the power level of the signals at different frequencies. The `Accelerometer` window will also scroll data.  

![Accel Moving](../assets/images/ganglion_moving-accelerometer.jpg)

Pick up your board, and move it around. You should see the data in the `Accelerometer` window also move around, and if you're touching the input pin headder, you will see some noise in the other windows. Nice!  

**NOTE If you're having trouble, check out the [troubleshooting](http://docs.openbci.com/Tutorials/02-Ganglion_Getting%20Started_Guide#ganglion-getting-started-guide-troubleshooting) section below.**

Now that you've got your computer connected to the Ganglion, it's time to connect your *self!*  



## Connect yourself to OpenBCI

In this quick demo, we'll be showing you how to set up your Ganglion to read 3 your heart activity (ECG), muscle activity (EMG), and brain activity (EEG)!

For more information on these three signals, refer to wikipedia:

 * [Heart Acitivity - Electrocardiography (ECG)](http://en.wikipedia.org/wiki/Electrocardiography)
 * [Muscle Acitivity - Electromyography (EMG)](http://en.wikipedia.org/wiki/Electromyography)
 * [Brain Activity - Electroencephalography (EEG)](http://en.wikipedia.org/wiki/Electroencephalography)

## Connect for ECG

Let's start off with something simple, ECG is the electric signal that causes your ticker to tick, and it's easy to measure if you attach electrodes on either side of your body.


![ECG Arms](../assets/images/ganglion_ECG-arms.png)

In this example, I'm attaching two of the sticky `SKINTACT` electrodes to either arm, and then an extra one on my elbow. It doesn't matter what elbow you choose.

![Ganglion Switches Differential](../assets/images/ganglion_SW_UP.png)

Now a note about your Ganglion board setup. There are 4 switches on the top of the board that are used to re-route the input connections to make connecting yourself easy. The default setting (the way your ganglion was shipped to you) is with the switches in the `UP` position. This allows you to connect your electrodes to the `+` and `-` pins of any channel, and measure the differential between them. For more of a deep dive on Ganglion Hardware, go to [this Doc](http://docs.openbci.com/Hardware/07-Ganglion)

![ECG connection TOP](../assets/images/ganglion_ECG-plugged-top-view.png)
![ECG connection PINS](../assets/images/ganglion_ECG-plugged-pins.png)

Here, I'm connecting my `arm` electrodes to the `+` and `-` pins of channel `3`.  

**NOTE Connect the `+` pin to your LEFT arm, otherwise the pulse wave will be upside down! The `+` pin is on the TOP row of the pin header. See the [Ganglion Hardware](http://docs.openbci.com/Hardware/07-Ganglion) doc for more details.**

You also need to connect the elbow electrode to the pin labeled `D_G` This is the `Driven Ground` pin of the Ganglion, and it is important to connect to this pin so that you and the Ganglion 'agree' on what `0 Volts` is, otherwise your signal will be unstable.

![channels on/off](../assets/images/ganglion_channels-ON-OFF.jpg)

Since we are only using channel `3` for this example, you can turn off the other channels so that they don't fill the screen with noise. Click on the channel number to turn off channels `1`, `2`, `4`. You can also turn them back on just by clicking the number.

![Ganglion ECG](../assets/images/ganglion_LIVE-ECG.jpg)

You should see on the `Time Series` window a waveform that is called a 'normal sinus rhythm'. That's your heart beat! If you don't see a waveform like the one on the right, then you might be a robot... One way to check to make sure that you are wired up to the Ganglion correctly is to do what's called an Impedance Check. This process will measure the connection quality between your body and the Ganglion.

![Change to Impedance Widget](../assets/images/ganglion_change-widget-to-impedance.jpg)

To measure your connection to the board, we have to change the Accelerometer widget into the Impedance widget. Click on the `Accelerometer` drop down menu and select `Ganglion Signal`. You will see a button labeled `Start Impedance Check`. Press that button.

![Measure Impedance](../assets/images/ganglion_ECG-impedance.jpg)

When you start the impedance check, the data will stop streaming, but some numbers will start to pop up in the `Ganglion Signal` window. These values are a measure of the input impedance, or the connection quality, between your body and the Ganglion. In the case of using ECG electrodes on bare skin, you would expect to see a value of between 5k and 10k. Notice the other channels are reporting high values. That's because there is nothing connected to them! Notice that the dot next to `Channel[3] Impedance` is green. That means it's good! The lower, the greener, the better!

## Connect for EMG

![EMG Arms](../assets/images/ganglion_EMG-fist.png)

Now, let's take a look at some EMG signals. EMG is the measure of the electrical activity of your muscles, and to do this, we will need to attach another of the `SKINTACT` electrodes. I'm sticking another one on my RIGHT wrist, and attaching the snap cable to it.

![EMG Signal](../assets/images/ganglion_EMG-signal.jpg)

The EMG signal is a high frequency signal that is really easy to see in the Time Series window. In this image, I'm squeezing my fist three times in a row.

## Connect for EEG

![Switches DOWN](../assets/images/ganglion_SW_DOWN.png)

Now, let's set up to see some brainwaves! The first thing you have to do is make an adjustment to the input switches. Remember, when we ship your Ganglion the switches `SW1, SW1, SW3, SW4` in the UP position, which allows you to connect to each channels `+` and `-` input pins. In this configuration, we say that these are "differential inputs". When the switch is in the DOWN position, the `-` pin is disconnected from the electronics, and that `-` input is connected instead to the `REF` pin. In this way, the switch helps you to gang together two or more of the `-` pins to use as a single reference. This scheme is useful when doing EEG, as you will soon see.  
So, First, switch all of the `SW` pins to the DOWN position.

![EEG pin connections](../assets/images/ganglion_EEG-plugged.jpg)

Next, connect the female header end of 6 of the Gold Cup Electrodes to the Ganglion input header. In this case, you want to be sure to connect to the `+` input, of channels 1, 2, 3, and 4, which is on the TOP row. You also need to connect one cable to the `REF` pin (either TOP or BOTTOM is ok) and also the `D_G` pin (either TOP or BOTTOM is ok).

![electrode paste scoop](../assets/images/electrodePaste.png)
![Connect REF & D_G paste](../assets/images/ganglion_connect-earlobe-paste.jpg)
![Connect Ref & D_G tape](../assets/images/ganglion_connect-earlobe-tape.jpg)

The first connection to make is the `D_G` electrode. This connection allows the Ganglion to 'share' `GROUND` or `0 Volts` with your body, so that we can measure the electo-potentials correctly. Scoop up a small amount of the eclectrode pasted with the gold cup (as shown). This paste acts as a kind of adhesive. It is also electrically conductive, and makes the connection between your skin and the gold cup. This connection will be on your ear lobe. It can help to have some medical tape or bandaid to help hold the electrode in place. Do the same thing with the gold cup electrode connected to the `REF` pin on your other earlobe. The `REF` pin is connected to all of the channel `-` inputs. This is the electrode that the ones on your head (reading your brain) will be measured against. We are attaching it to your earlobe, because there is *very little* electrical signal in your earlobe, so it won't interfere with what's going on in your head.

![10-20 map positions](../assets/images/ganglion_10-20-positions.png)

It's important to know where you are placing your EEG electrodes on your head, and thankfully there already is a map of electrode positions. It's called the [10-20 system](https://en.wikipedia.org/wiki/10-20_system_(EEG)). In the picture  at right, the Nasion is the 'nose' side of your head, and the Inion is the 'back' side of your head. I have color coded the electrode positions for you, based on the cables connected in previous image, and you can see that we've already applied the `D_G` and `REF` at positions `A2` and `A1` respectively.

![Electrode Frontal Place](../assets/images/ganglion_frontal-place.jpg)
![Electrode Frontal Position](../assets/images/ganglion_frontal-position.jpg)

The positions `Fp1` and `Fp2` are your Frontal Parietal positions. They should be placed semetrically on your forehead as shown in the picture. `Fp1` should connect to Channel 1, and `Fp2` should connect to Channel 2. I'm using the same color electrode wires as is used in the GUI channel color.

![Electrode Occipital Place](../assets/images/ganglion_occipital-place.jpg)
![Electrode Occipital Position](../assets/images/ganglion_occipital-position.jpg)

Channel 3 and Channel 4 should be connected to your head in the `O1` and `O2` positions. These are going to measure your Occipital lobe (Connected to your eyes!). make sure to part the hair, and get the electrode connected right on to your scalp. It can help to have a friend do this part with you. *VERY* important to make the connection to your scalp! use more electrode paste if you need to.

![Electrodes Banded GtoG](../assets/images/ganglion_electrodes-ready.jpg)

I'm using a headband to help hold the electrodes in place, and now I'm good-to-go! Let's check out some EEG!

![GUI Adjust for EEG](../assets/images/ganglion_vert-scale-50.jpg)

Start the GUI as you have done before, and this time, set the `Vert Scale` to `50uV`.

![Eye Blinks!](../assets/images/ganglion_EEG-eye-blinks.jpg)

Press the `Start System` button, and give the data a moment to settle. The first fun thing to measrue is eye blinks. If you blink your eyes, you will see a signature wave in the EEG signal on Channel 1 and Channel 2.

![Jaw Grits](../assets/images/ganglion_EEG-jaw-grits.jpg)

Next, let the signal settle again and then grit your teeth just a bit. You should be able to see some nice EMG from your jaw muscles in two or more of the channels.

![Alpha!](../assets/images/ganglion_EEG-alpha.jpg)

Finally, let's try to get some brainwaves! The easiest brainwave to make 'on command' is an alpha wave. In most of our waking life, our eyes are open and the occipital lobe of our brains is busy processing all of the visual information streaming onto our retinas. It just so happens that when you close your eyes, your occipital lobe has 'nothing to do' as it were, and goes into an 'idle' state. In this state, it produces a brainwave at about 10Hz (between 8Hz and 12Hz). You can measure the alpha wave with the Ganglion when your eyes are closed. So now, close your eyes, and have your friend watch the GUI for signs of alpha. You should see a dominant waveform in the `Time Series` window, and a rising peak in the `FFT Plot` at about 10Hz. Well, you won't see it, because you have your eyes closed! But your friend who helped you put the electrodes on will see it!  

![EEG Impedance Test](../assets/images/ganglion_EEG-impedance-test.jpg)

If you having any trouble seeing the signals above, one thing that might be an issue is the connection between the gold cup electrodes and your scalp. You can test this connection by doing an Impedance Check. Click the button `Start Impedance Check` and you will see values start to come up at each electrode. The small circle on the left will change color according to the impedance, with `green` being good and `red` being not-good. Using gold cup electrodes and paste, you should be seeing impedance values in the range of `5k` to `15k`. If they are higher, you will need to adjust the connection, add more paste and re-position the electrode if necessary.


**Happy Brain Hacking!**





## RUN THE GUI ON macOS SIERRA


When Apple Computer updated their Operating System to Sierra (v10.12.x), they changed a few things about your `Security & Privacy` default settings. Sierra won't allow any apps that aren't from the App Store or Identified Developers. While we work on becoming Identified Developers, you will need to change your default `Security & Privacy` settings. Here's how to do it:  

![sudo](../assets/images/ganglion_sudo-command.png)

1. Open the Terminal app from your /Applications/Utilities/ folder and then enter the following command syntax: `sudo spctl --master-disable` and press the  `return` key.
2. You will be prompted to enter your administrator password. Do that, and then press `return` key.

>This hack was published by [osXdaily](http://osxdaily.com/2016/09/27/allow-apps-from-anywhere-macos-gatekeeper/) September, 2016.

![Allow Apps](../assets/images/ganglion_SysPrefs-Allow.png)

Now, go to your `System Preferences/Security & Privacy` and make sure that your system allows apps downloaded from Anywhere. You may again be prompted for your administrator password.   
Now go back to where you were before to continue!

##TROUBLESHOOTING

If the initialization and data stream fails, try the following steps:

1. Make sure your computer's Bluetooth is turned `ON`
2. Making sure you've selected the correct Ganglion, if there are multiple Ganglions in the viscinity.
3. Power down your Ganglion, and close the GUI. Then try restarting the system, buy turning on the Ganglion, and restaring the GUI.
4. Make sure that your batteries are fully charged and then retry the steps above.
5. If you are still having troubles connecting to your OpenBCI board, refer to the [Forum](http://openbci.com/index.php/forum/) for extra troubleshooting advice.
