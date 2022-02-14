# Sharek
Buy/Sell assets in cash/crypto based on smart contracts


## Installing Binary Distribution, Building from Source and Starting Besu

### Installing Binary Distribution
If you are using Mac OS, you need to have Homebrew and Java JDK to get started. You also need Java 11+ as earlier Java versions are not supported.

Now, run the following command to install using Homebrew.

```brew tap hyperledger/besu```

```brew install besu```

To check if Besu is installed successfully, check with the following command.

```besu –help```

If you are using Unix/Linux/Windows, then you to download Besu packaged binaries. Once downloaded, unpack the files and go to the besu-<release> directory. 

To confirm that Besu is installed correctly, use the besu –help command.

  
### Build from Source
  
To build Besu from the source, you need to clone the Besu repository.

```git clone –recursive https://github.com/hyperledger/besu.git```

Once the cloning is done, we will eliminate tests using the following command:

```./gradlew build -x test```

Now, go to the distribution directory using the command:

```cd build/distributons/```

From there, you need to expand the distribution archive using the following command.

```tar -xzf besu-<version>.tar.gz```

With the files expanded, now move to the new folder.

```cd besu-<version>/```

```bin/besu –help```

If the last command runs successfully, you have successfully build from source.

For Windows, the process is almost the same. You start by cloning repository, removing tests, going to distribution directory, expanding it, and then finally checking if the installation is successful or not.

