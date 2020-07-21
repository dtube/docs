### How to create a custom key

In order a create a custom key, you need to enter your **channel** then go into **keys**

<center>

![](https://i.imgur.com/aJTzTX3.png)

</center>

#### Key identifier
This one can be any word you want. It's to remember what the key is for later on.

#### New keypair
You need to store your **private** key somewhere safe you can store it as image by using QR or you can save it as a file.
**Cryptographic keys cannot be recovered**, however, if you have your master key safe already, it will always be possible to remove the "forgotten" custom key and create a new one in place. So it is less important for those custom keys to be stored redundantly.

#### New key permissions
After that you need to choose which transaction types the key will be allowed to use. If you want to create a custom key for casual browsing and that cannot access your funds, we recommend you to allow all those permissions:
* APPROVE_NODE_OWNER
* DISAPROVE_NODE_OWNER
* COMMENT
* VOTE
* USER_JSON
* FOLLOW
* UNFOLLOW

### How to safely store your private keys
The master key is the most important one, and should be stored redundantly (with at least 1 backup). Any custom key with access to your funds should also be safe, but doesn't need redundancy as your master key would always allow you to reset your custom key to a new one if ever lost.

Good examples of safe storage, can be a USB stick, a piece of paper, or a device that does not connect to internet.

Bad example of how to store a private key: sending yourself an email with the key in plain text, cloud storage solutions (google drive, iCloud), the desktop of your family PC.

### Encrypting your master key
It's also strongly recommended to encrypt your master key before storing it (e.g. on a USB stick).

[Encrypt a file using Windows](https://support.microsoft.com/en-au/help/4026312/windows-10-how-to-encrypt-a-file)

[Encrypt a file using MacOs](https://blog.macsales.com/47804-in-the-vault-how-to-encrypt-files-on-your-mac/#:~:text=Go%20to%20the%20File%20menu,the%20new%20encrypted%20disk%20image.)

### Changing my master key
This one is also in My Channel -> Keys. Be extra careful when using this one, and make sure that you properly saved the key before changing it. There will be no way to go back to the old master key. If you current master key has no reason to be compromised, there is little reason to change it.
