# KORTHO
## 下载地址
| windows | linux |
|  :----  | :----  |
|  [0.0.1](https://www.kortho.org/file/windows/1.zip)  | [0.0.1](https://www.kortho.org/file/linux/1.zip) |

    
## 配置安装：
### windows下：
        第一步 在工作目录下创建挖矿目录，如 D:/miner（非C盘）。

        第二步 将windows 下载的挖矿软件包解压到D:/miner下。

        第三步 进入生成的解压目录，修改config下"korthoConf.yaml"的配置文件（**非常关键的一步）：
            （1）：找到'Miner'参数修改为自己的矿工地址，如 Miner : "Kto***"。

        第四步 进入生成的解压目录，打开windows命令行：        
            （0）：键入命令:
```
                ./miner.exe -n 100 -b 0x20002000 -s 1 -m 2
             
```
            （1）：-n 表示
            （2）：-b 表示
            （3）：-s 表示
            （4）：-m 表示

        第五步 回车执行命令，开启挖矿。

        第六步 查询挖矿：打开自己的矿工钱包，查询挖矿情况。

### linux下：

        第一步 在工作目录下创建挖矿目录，如 /work/miner。

        第二步 将 linux 下载的挖矿软件包解压到/work/miner下。

        第三步 进入生成的解压目录，修改config下"korthoConf.yaml"的配置文件（**非常关键的一步）：
            （1）：找到'Miner'参数修改为自己的矿工地址，如 Miner : "Kto***"。

            （2）：键入命令:
```
                sudo ./miner -n 100 -b 0x20002000 -s 1 -m 2
             
```             
            （3）：-n 表示
            （4）：-b 表示
            （5）：-s 表示
            （6）：-m 表示

        第四步 回车执行命令，开启挖矿。

        第五步 查询挖矿：打开自己的矿工钱包，查询挖矿情况。

## 源码安装：
        不管linux或是windows环境，首先要保证安装了go环境。

### windows下：
            第一步 编译源码：            
                （0）：在工作目录下创建挖矿目录，如 D:/miner，然后在miner下创建config目录。
                （1）：进入源码目录，打开windows命令行执行：go env -w GOOS=windows|go build -o .\miner.exe .\main.go。

            第二步 进入miner目录，将生成的miner.exe 拷贝当前目录下，再将源码pkg/config/korthoConf.yaml拷贝到当前/config目录下。

            第三步 修改/miner/config下"korthoConf.yaml"的配置文件（**非常关键的一步）：            
                （1）：找到'Miner'参数修改为自己的矿工地址，如 Miner : "Kto***"。

            第四步 进入miner目录,打开windows命令行：
                （0）：键入命令: 
```
                    ./miner.exe -n 100 -b 0x20002000 -s 1 -m 2

```
                （1）：-n 表示
                （2）：-b 表示
                （3）：-s 表示
                （4）：-m 表示

            第五步 回车执行命令，开启挖矿。

            第六步 查询挖矿：打开自己的矿工钱包，查询挖矿情况。

### linux下：
            第一步 编译源码：
                （0）：在工作目录下创建挖矿目录，如 /work/miner，然后在miner下创建config目录。
                （1）：进入源码目录，在命令行执行：go build -o /work/miner .\main.go。

            第二步 进入miner目录，将源码pkg/config/korthoConf.yaml拷贝到/work/miner/config目录下。

            第三步 /work/miner/config，修改"korthoConf.yaml"的配置文件（**非常关键的一步）：
                （1）：找到'Miner'参数修改为自己的矿工地址，如 Miner : "Kto***"。

            第四步 /work/miner/：
                （0）：键入命令: 
```
                    sudo ./miner -n 100 -b 0x20002000 -s 1 -m 2

```
                （1）：-n 表示
                （2）：-b 表示
                （3）：-s 表示
                （4）：-m 表示

            第五步 回车执行命令，开启挖矿。

            第六步 查询挖矿：打开自己的矿工钱包，查询挖矿情况。
