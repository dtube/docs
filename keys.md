## Public Key vs Private Key
When adding a new key to DTube, you will be shown a public key, and a private key.

The public key is what will be linked to your username in the public blockchain data. Everyone will be able to see your public key. In other blockchains like Bitcoin, you would use the Public key as the destination address for a monetary transfer, however on d.tube, everyone has a username, so we use the username for monetary transfers instead.

The private key is the part you are supposed to keep private to yourself. It's the one you will use for login and that permits you to do any operation on the chain.

### A private key is not like a password
Unlike your password on facebook or gmail, a private key can NOT be recovered if you lose it.

## Master Key vs Custom Keys
DTube accounts can have multiple keys associated to it: 
* The first one is the **master** key, which can fully control the account. It can do any type of transaction, including creating and deleting new keys, or changing the master key. Your DTube account always has only one master key.
* Second one is called **custom** keys. They can be created by the master key, and are granted lower permissions based on transaction types. You can for example create a key, which is only permitted to vote, follow, or comment. This key would therefore not be able to use the DTCs in your account, and you not put your funds at risk if it got hacked/stolen. Your account can have many customs keys.

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

