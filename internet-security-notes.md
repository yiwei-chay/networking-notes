# mTLS (Mutual Transport Layer Security)

## 1. What is mTLS?
mTLS (Mutual Transport Layer Security) is a process of mutual authentication to ensure that both parties at each end of the network connection are verifying that they each hold the correct private key. Additional verification is provided through their respective TLS certificates - a protocol for encrypting Internet traffic and verifying server identity.

### 1.1 Advantages of mLTS
- **Improved Security**: mTLS encrypts all data transmitted over the connection
- **Reduced Complexity**: mTLS simplifies security architecture by eliminating the need for separate authentication mechanisms

### 1.2 How does mTLS work?
In mTLS, both the client and the server possess a certificate and can authenticate using their public/private key pair. There is the need to verify both parties before the exchange of information takes place. The steps in which mTLS operates are outlined as follows:
1. Client connects to the server
2. Server presents its TLS certificate
3. Client verifies the server's certificate
4. Client presents its own TLS certificate
5. Server verifies client's TLS certificate
6. Access is granted by the server 
7. Both parties exchange information over encrypted TLS connection


## 2. Questions
### 2.1 How is mTLS different from what has been described in this lecture (securing websites)?
mTLS is an extension of TLS; apart from the server just presenting the TLS certificate, the client in mTLS also issues a TLS certificate to establish its identity. The TLS handshake hence contains several extra steps before exchange of information takes place.

### 2.2 Where is mTLS frequently used?
mTLS is more frequently used on a smaller scale - for individual organisations who employ a Zero Trust approach to network security. The Zero Trust approach does not trust any user, device, or request. mTLS allows authenticating users and verifying devices every time they try to request to access any point in the network.

### 2.3 Give an example application which uses mTLS
Zero Trust Security.

### 2.4 Draw a diagram to show the process
Steps references instructions from Section 1.2.
![image](https://github.com/yiwei-chay/networking-notes/assets/146081571/f4a7e362-69ab-40c8-a3bf-893146206290)

