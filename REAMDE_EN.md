# KORTHO
## download
|windows | linux |
|  :----  | :----  |
|  [0.0.1](https://www.kortho.org/file/windows/miner_windows_001.zip)  | [0.0.1](https://www.kortho.org/file/linux/miner_linux_001.zip) |

## deploy
### windows
        1. Create a mining directory under the working directory,like D:/miner（not C:/）.

        2. Unzip the package into D:/miner.

        3. go into decompressed directory，modify the "korthoConf.yaml" under config（**A very important step）：
            （0）：Find 'Miner',fill in your miner's address。

        4. Open the Windows command line：        
            （0）：Command:
```
                ./miner.exe -n 100 -b 0x20002000 -s 1 -m 2
             
```
            （1）：-n means
            （2）：-b means
            （3）：-s means
            （4）：-m means

        5. Press Enter to run the command to start mining.

        6. Query mining: Open your miner's wallet and query mining.

### linux

        1. Create a mining directory,like /work/miner。

        2. Unzip the package into D:/miner.

        3. go into decompressed directory，modify the "korthoConf.yaml" under config（**A very important step）：
            （0）：Find 'Miner',fill in your miner's address。
            （1）：Command:
```
                sudo ./miner -n 100 -b 0x20002000 -s 1 -m 2
             
```             
            （2）：-n means
            （3）：-b means
            （4）：-s means
            （5）：-m means

        4. Press Enter to run the command to start mining.

        5. Query mining: Open your miner's wallet and query mining.

