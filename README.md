# proveLOC demo

# TL;DR
[Webapp](https://proveloc-11543.firebaseapp.com/): Add source code verification for given URL

[Chrome extension](https://mega.nz/#!6zQTXIIB!UHqe3Di2izpf3ZkL581NwA1_fg6l7HDSvpcbW4o2XR8): Verify loaded scripts for given URL. (Install by drag-and-drop to [chrome://extensions](chrome://extensions))

Sample URLs with verified source code: 

- https://www.fh-kufstein.ac.at/
- http://www.kufstein.at/
- http://www.stefanhuber.at/

# Usage

You can use the web app and the chrome extension of proveLOC. The smart contracts are deployed to the [Ropsten Testnet](https://ropsten.etherscan.io/address/0xdc8cb1f6fe73be5f52648f502ff8d85ef2a267d8). 

### Preqreuisites
  - [MetaMask](https://metamask.io/)
  - Chromium Browser
  - Create Account in Metamask, select Ropsten Test Network and request some free Ether [here](https://faucet.metamask.io/)

### Webapp
The web app is [deployed on firebase](https://proveloc-11543.firebaseapp.com/).
Use the web app to add proofs for a given URL (simply add the source files to verify them).

### Chrome Extension

#### Installation
- Download the Chrome extension from [here](https://mega.nz/#!6zQTXIIB!UHqe3Di2izpf3ZkL581NwA1_fg6l7HDSvpcbW4o2XR8).
- Install the Chrome extension by opening [chrome://extensions](chrome://extensions) in your browser and drag and drop the zip archive to that tab

#### Usage
Visit one of the demo URLs with verified source code and click on the extension icon: 

- https://www.fh-kufstein.ac.at/
- http://www.kufstein.at/
- http://www.stefanhuber.at/


# Known issues
 - sometimes a reload of the page is necessary for the inline sources to load properly. This might be due to a problem with the chrome debugger events - further investigation is necessary.
 - sometimes the debugger does not properly detach / disable when closing the popup (although this might be solved already)

# Limitations
This prototype does not (and wasn't planned to) cover the following subjects:
 - Proper error handling
 - Form field verification
 - Usability and Design
 - Custom version number
 - Code verification might not work when there are certain special characters in the code (anyhting that results in a different hash breaks it of course)

# Contact
Feel free to reach out to benedikt.berger@live.de
