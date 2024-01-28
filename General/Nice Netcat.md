Nice Netcat is about using a `netcat` connection to receive data.
```
nc [address] [port]
```

1. Use the given `netcat` command given in the description of the challenge

When using `netcat` you can use the abbreviation nc.

Nc creates a connection with a port using a TCP and UDP process to read and write data across a network.

2. Once connected, decrypt the decimal data to ASCII

When connecting to the `nc` socket, a bunch of decimal numbers are sent across the stream to us. 

Assuming that these numbers correlate to the flag, we can try to decrypt using the ASCII system

The ASCII system is the American Standard Code for Information Interchange. This maps all characters to decimal digits so that computers can read it. It was originally made for encryption uses and so that computes could communicate internationally.

Once we copy these decimals to ASCII, it spells out the flag for us!