# How does D.Tube work?
              `

## Using the Avalon Blockchain as a database

Because we want D.Tube to be truly decentralized, we cannot have a server running a database and use it to query things. Using Avalon blockchain is a natural solution. . It is fast . It is free, anyone can use it without having to deposit some form of currency, and transactions have no fees. Who would want to pay money to upload a video, comment a video, or even upvote? Nobody. Any video uploaded on D.Tube becomes an Avalon content, that can earn rewards also you can post your content to Steem and Hive blockchains and benefit from interoperable features of Dtube.


 **Using IPFS as a static file storage**


<center>![](https://i.imgur.com/uDThjEm.png)</center>

 IPFS is a protocol that enables decentralized file storage. The principle behind it is called Distributed Hash Tables (DHT). The same principle also powers the BitTorrent network. Just like how cryptocurrency uses asymmetrical cryptography, DHT networks will hash contents in order to be able to identify a file. The hash becomes the identifier of a file, and it's as easy as re-hashing a file and making sure the hashes match to ensure the file that was sent to us is the original.

Why not use Torrent then? Torrent arguably already has more content and is more mainstream. However, Torrent was not built for the web. Some implementations such as WebTorrent are trying to make it work, but it still requires some 'hybrid' clients that would act as bridges in order to transfer files from hard clients such as μTorrent to web clients that run in a browser. Not very convenient, even less efficient. I am sure a lot of you have used PopcornTime to watch some 'pirated' content and have enjoyed it, but building something similar that runs inside a browser without having to run hybrid clients to connect people, is sadly impossible.
IPFS is a younger, open-source, and actively developed protocol. It has a bright future ahead. Using it as the main mean of storage for this project was a no-brainer.`
