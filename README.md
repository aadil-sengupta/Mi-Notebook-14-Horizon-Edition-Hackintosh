# Mi-Notebook-14-Horizon-Edition-Hackintosh

This repositery is a Documentation / Guide on how to install macOS on the Mi Notebook 14 Horizon Edition. The below Guide I prepared a simple way on how you can get started with a hackintosh on your Mi Notebook 14 Horizon edition, This guide not only talks about the basic installation steps but also talks about the problems that you are to encounter during the installation process


## OpenCore Version: 7.6

# So, Lets Begin!

First lets talk about what works and what dosent
As of right now evreything that you would expect works,

|   Features     | Status |
| ----------------- | :----:  | 
| Touchpad Gestures |   ✅    |
| Keyboard          |   ✅    |
| Audio             |   🟢    |
| Microphone        |   🟨    |
| Wifi              |   ✅    |
| Bluetooth         |   ✅    |
| Sleep             |   🟢    |
| Power Management  |   ✅    |
| Dgpu Disable      |   ✅    |
| USB Map           |   ✅    |
| Handoff           |   ✅    |
| Sidecar           |   ✅    |
| HDMI              |   ✅    |
| Airdrop           |   🔴    |

<details>
  <summary>Config</summary>
  
</details>

# Installation

### Note:-
This EFI is meant for the Mi Notebook 14 Horizon Edition and while it can work on the non-Horizon edition, things such as sleep, Wifi, Dgpu disable, etc. might not work. Those trying to hackintosh the Non-Horizon version can Try using this one or tweak this EFI to suit you needs.<br>
<br>First We need to download macOS, to do so, we have a few options. I reccomend that you download a offline installer as installing macOS via the online installer has caused issues due to our wifi card. Another thing to note here. If you want to use apple services such as Imessaegs & Facetime. You will need to install Catalina first and then upgrade to Monterey or Big sur. Also, if you want to make things a bit easy, Please directly install Monterey. though Imessages wont work, its a much simpler process as i encountered several issues while upgrading from catalina to big sur & from big sur to Monterey.

* [Using a real Mac](#real)
* [Olarila image](#img)
* [gibMacOS](#gib)

<a name="real"></a>
<details>
<summary>Using a real Mac</summary>
  
  On a real Mac (a functional hackintosh will do as well) Download the installer for the desired version of macOS from the app store using the following links:-<br>
<br>[BigSur](https://apps.apple.com/us/app/macos-big-sur/id1526878132?mt=12) <br>
[Monterey](https://apps.apple.com/us/app/macos-monterey/id1576738294?mt=12)<br>
[Catalina](https://apps.apple.com/sg/app/macos-catalina/id1466841314?mt=12)<br>
  <br>
Now, Insert your flash drive(14gb or more) open a terminal window and type the following depending on the macOS version you downloaded:-

  
      BigSur
      sudo /Applications/Install\ macOS\ Big\ Sur.app/Contents/Resources/createinstallmedia --volume /Volumes/MyVolume

      Catalina
      sudo /Applications/Install\ macOS\ Catalina.app/Contents/Resources/createinstallmedia --volume /Volumes/MyVolume

      Monterey
      sudo /Applications/Install\ macOS\ Monterey.app/Contents/Resources/createinstallmedia --volume /Volumes/MyVolume
  
</details>
