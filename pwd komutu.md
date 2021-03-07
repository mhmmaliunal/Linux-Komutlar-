# pwd

> pwd komutu (Print Working Directory), temel olarak terminal üzerinde içinde bulunduğunuz klasörün yolunu gösterir.

<code><pre>
demo@demo-pc:~/Documents/Github Tutorials/Linux Tutorials$ pwd
/home/demo/Documents/Github Tutorials/Linux Tutorials
</code></pre>

Yukarıda görüldüğü gibi pwd komutu içinde bulunduğumuz klasörün yolunu tam olarak bize gösterdi. Pwd komutunun yardım ve versiyon opsiyonları hariç iki opsiyonu vardır. Bunlar -P ve -L dir.

- <code>__*pwd -L*__</code> <br/>
Doğrudan fiziksel olarak içinde bulunduğunuz klasörün yolunu döndürür. Sembolik linklerden kaçınır. Eğer bir opsiyon belirtilmemiş ise pwd komutu varsayılan olarak bu opsiyon ile aynı sonucu döndürür.
- <code>__*pwd -P*__</code><br/>
Bu komut eğer içinde bulunduğunuz klasör bir kısayol klasörü ise - yani ana klasörden ayrı bir klasöre link verilerek oluşturulmuş bir klasör ise - asıl klasörün tam yolunu döndürür.

Aşağıdaki kullanımın örnekleri için bir açıklama yapmak gerekirse: workingdir klasörü içinde bulunan linkingFolder gerçek bir klasör ve bu klasör için Desktop klasöründe wd isimli bir kısayol klasörü oluşturulmuştur. *terminal 1* örneğinde komutun ve opsiyonlarının gerçek klasör üzerindeki çıktıları görülmketedir. *terminal 2* örneğinde ise sembolik lik verilerek oluşturulmuş kısayol klasöründe komutun ve opsiyonlarının çıktıları görülmketedir 

<code>terminal 1:<br/><pre>
demo@demo-pc:~/Documents/Github Tutorials/Linux Tutorials/workingdir/linkingFolder$ pwd
/home/demo/Documents/Github Tutorials/Linux Tutorials/workingdir/linkingFolder
demo@demo-pc:~/Documents/Github Tutorials/Linux Tutorials/workingdir/linkingFolder$ pwd -P
/home/demo/Documents/Github Tutorials/Linux Tutorials/workingdir/linkingFolder
demo@demo-pc:~/Documents/Github Tutorials/Linux Tutorials/workingdir/linkingFolder$ pwd -L
/home/demo/Documents/Github Tutorials/Linux Tutorials/workingdir/linkingFolder
</code></pre>

<code>terminal 2:<br/><pre>
demo@demo-pc:~/Desktop/wd$ pwd
/home/demo/Desktop/wd
demo@demo-pc:~/Desktop/wd$ pwd -P
/home/demo/Documents/Github Tutorials/Linux Tutorials/workingdir/linkingFolder
demo@demo-pc:~/Desktop/wd$ pwd -L
/home/demo/Desktop/wd
</code></pre>

# /bin/pwd

> *pwd* komutu ile aynı işlevi görür. Tek fark opsiyon kullanılmayan komutların davranışlarıdır. *pwd* komutu varsayılan olarak *pwd -L* komutu ile aynı çıktıyı verirken, */bin/pwd* komutu */bin/pwd -P* komutu ile aynı çıktıyı verir.

<code><pre>
demo@demo-pc:~/Desktop/wd$ /bin/pwd
/home/demo/Documents/Github Tutorials/Linux Tutorials/workingdir/linkingFolder
demo@demo-pc:~/Desktop/wd$ /bin/pwd -P
/home/demo/Documents/Github Tutorials/Linux Tutorials/workingdir/linkingFolder
demo@demo-pc:~/Desktop/wd$ /bin/pwd -L
/home/demo/Desktop/wd
</code></pre>

Kaynak linki:[ET 29.01.21]<br/>
[https://www.geeksforgeeks.org/pwd-command-in-linux-with-examples/](https://www.geeksforgeeks.org/pwd-command-in-linux-with-examples/)