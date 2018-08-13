# -
服务器性能测试脚本
偶然在LET看到的一个歪果仁用的测试脚本
Github
另一个脚本也可以关注：Caddy Web Server 一键安装
使用
curl -LsO git.io/bench.sh; chmod +x bench.sh
./bench.sh -b shareCopy
参数解释
Usage
./bench.sh Arguments Parameters (Optional)Copy
Arguments
-info # System Information
-io # I/O Test
-cdn # CDN Download (200MB)
-northamerica # North America Download (800MB)
-europe # Europe Download (900MB)
-asia # Asia Download (400MB)
-b # System Info + CDN Download + I/O Test
-a # All In One Command
-speed # Test from speedtest.net using speedtest cli
-help # Show help
-about # Show aboutCopy
Parameters – Share
例子 : ./bench.sh -cdn share haste

可选项:
ubuntu 
# upload results to ubuntu paste (default)
haste 
# upload results to hastebin
clbin 
# upload results to clbin
ptpb
# upload results to ptpbCopy
Credits
Thanks to @camarg for the the original script. Thanks to @dmmcintyre3 for the modified version. Thanks @Hidden_Refuge for update bench-sh-2.Copy
演示
# curl -LsO git.io/bench.sh; chmod +x bench.sh
# ./bench.sh -b share

 Benchmark started on 18-May-2018 12:05:46

 ## System Information

 OS Name     : Debian GNU/Linux 8.10 (jessie) (64 bit)
 Kernel      : Dedicated / 4.16.3-041603-generic
 Hostname    : blog.liyuans.com
 CPU Model   : Intel(R) Core(TM) i3-2130 CPU @ 3.40GHz
 CPU Cores   : 4 cores @  2644.868 MHz
 CPU Cache   : 3072 KB
 Total RAM   : 7876 MiB (Free 1460 MiB)
 Total SWAP  : 4094 MiB (Free 4080MiB)
 Total Space : 1.8TB (1% used)
 Running for : 16days - 21hrs 05min 44sec


 ## CDN Speedtest

 CacheFly :  10.82 MiB/s |   86.58 Mbps  | ping   7.414ms
 CDN.net  :   9.73 MiB/s |   77.84 Mbps  | ping  18.013ms
 Gdrive   :   6.74 MiB/s |   53.96 Mbps  | ping  13.593ms


 ## IO Test

 CPU Speed:
    bzip2 512MB -  95.7 MB/s
   sha256 512MB -   154 MB/s
   md5sum 512MB -   512 MB/s

 Disk Speed (512MB):
   I/O Speed  - 610 MB/s
   I/O Direct - 13.2 MB/s

 RAM Speed (1024MB):
   Avg. write - 3379.2 MB/s
   Avg. read  - 5495.5 MB/s

 Benchmark finished in 115 seconds
   results saved on /root/bench.log

