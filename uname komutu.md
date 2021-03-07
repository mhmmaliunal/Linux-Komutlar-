# uname
---
- <code>__*uname*__</code> <br/>
Sadece kernel adını döndürür.
- <code>__*uname -s*__</code><br/>
Kernel adını döndürür.
- <code>__*uname -r*__</code><br/>
Kernel Release ini döndürür.
- <code>__*uname -v*__</code><br/>
Kernel sürümünü döndürür.
- <code>__*uname -n*__, __*uname --nodename*__</code><br/>
Bilgisayarın hostname ini döndürür.
- <code>__*uname -m*__</code><br/>
Donanım mimarisini döndürür.
- <code>__*uname -p*__</code><br/>
İşlemci tipini döndürür.
- <code>__*uname -i*__</code><br/>
Donanım platformunu döndürür
- <code>__*uname -o*__</code><br/>
İşletim sistemi adını döndürür.
- <code>__*uname -a*__</code><br/>
Tüm sistem bilgisini döndürür.
<br/>
<br/>
<code><pre>
demo@demo-pc:~$ uname
Linux
demo@demo-pc:~$ uname -s
Linux
demo@demo-pc:~$ uname -r
5.3.0-26-generic
demo@demo-pc:~$ uname -v
#28~18.04.1-Ubuntu SMP Wed Dec 18 16:40:14 UTC 2019
demo@demo-pc:~$ uname -n
demo-pc
demo@demo-pc:~$ uname --nodename
demo-pc
demo@demo-pc:~$ uname -m
x86_64
demo@demo-pc:~$ uname -p
x86_64
demo@demo-pc:~$ uname -i
x86_64
demo@demo-pc:~$ uname -o
GNU/Linux
demo@demo-pc:~$ uname -a
Linux demo-pc 5.3.0-26-generic #28~18.04.1-Ubuntu SMP Wed Dec 18 16:40:14 UTC 2019 x86_64 x86_64 x86_64 GNU/Linux
</code></pre>

Kaynak linki:[ET 23.01.21]<br/>
[https://vitux.com/get-debian-system-and-hardware-details-through-the-command-line/](https://vitux.com/get-debian-system-and-hardware-details-through-the-command-line/)