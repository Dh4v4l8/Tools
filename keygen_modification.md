```
hello@hello-friend:~/Desktop/burp2$ java -jar cfr.jar BurpLoaderKeygen.jar --outputdir decompiled
Processing BurpLoaderKeygen.jar (use silent to silence)
Processing com.h3110w0r1d.json.JSONParse
Processing com.h3110w0r1d.json.ParseResult
Processing com.h3110w0r1d.json.JSONType
Processing com.h3110w0r1d.json.JSONObject
Processing com.h3110w0r1d.burploaderkeygen.Keygen
Processing com.h3110w0r1d.burploaderkeygen.Loader
Processing com.h3110w0r1d.burploaderkeygen.Filter
Processing com.h3110w0r1d.burploaderkeygen.KeygenForm
```
```
hello@hello-friend:~/Desktop/burp2$ cd decompiled
```
```
hello@hello-friend:~/Desktop/burp2/decompiled$ find . -name "KeygenForm.class" -o -name "KeygenForm.java"
./com/h3110w0r1d/burploaderkeygen/KeygenForm.java
```
```
hello@hello-friend:~/Desktop/burp2/decompiled$ gedit /com/h3110w0r1d/burploaderkeygen/KeygenForm.java
```
```
hello@hello-friend:~/Desktop/burp2/decompiled$ ls
com summary.txt
```
```
hello@hello-friend:~/Desktop/burp2/decompiled$ gedit ./com/h3110w0r1d/burploaderkeygen/KeygenForm.java
```
```
File में निम्न changes करें:                                                                                               
                                                                                                                     
Line ढूंढें: frame = new JFrame("Burp Suite Pro Loader & Keygen Modified By h3110w0r1d v1.4");                                    
इसे बदलें: frame = new JFrame("Burp Suite Pro Loader & Keygen Modified By BlockBreach v1.4");
Line ढूंढें: text_license_text = new JTextField("licensed to h3110w0r1d");
इसे बदलें: text_license_text = new JTextField("licensed to BlockBreach");
```
```
hello@hello-friend:~/Desktop/burp2/decompiled$ javac -cp "../BurpLoaderKeygen.jar" com/h3110w0r1d/burploaderkeygen/KeygenForm.java
```
```
hello@hello-friend:~/Desktop/burp2/decompiled$ jar xf ../BurpLoaderKeygen.jar META-INF/MANIFEST.MF
```
```
hello@hello-friend:~/Desktop/burp2/decompiled$ jar cmf META-INF/MANIFEST.MF ../BurpLoaderKeygen_modified.jar -C . .
```
```
hello@hello-friend:~/Desktop/burp2/decompiled$ java -jar ../BurpLoaderKeygen_modified.jar
Success: '/usr/lib/jvm/java-21-openjdk-amd64/bin/java' can execute!
Exception in thread "main" java.lang.NoClassDefFoundError: com/h3110w0r1d/burploaderkeygen/Keygen
at com.h3110w0r1d.burploaderkeygen.KeygenForm.main(KeygenForm.java:431)
Caused by: java.lang.ClassNotFoundException: com.h3110w0r1d.burploaderkeygen.Keygen
at java.base/jdk.internal.loader.BuiltinClassLoader.loadClass(BuiltinClassLoader.java:641)
at java.base/jdk.internal.loader.ClassLoaders$AppClassLoader.loadClass(ClassLoaders.java:188)
at java.base/java.lang.ClassLoader.loadClass(ClassLoader.java:526)
... 1 more
```
```
hello@hello-friend:~/Desktop/burp2/decompiled$ cd ..
```
```
hello@hello-friend:~/Desktop/burp2$ ls
BurpLoaderKeygen.jar cfr.jar fernflower
BurpLoaderKeygen_modified.jar decompiled
```
```
hello@hello-friend:~/Desktop/burp2$ # पहले original JAR को extract करें
mkdir extracted_original
cd extracted_original
jar xf ../BurpLoaderKeygen.jar
# Decompiled class file को extracted directory में copy करें
cd ..
cp decompiled/com/h3110w0r1d/burploaderkeygen/KeygenForm.class extracted_original/com/h3110w0r1d/burploaderkeygen/
# नया JAR बनाएं
cd extracted_original
jar cmf META-INF/MANIFEST.MF ../BurpLoaderKeygen_fixed.jar .
cd ..
```
```
hello@hello-friend:~/Desktop/burp2$ ls
BurpLoaderKeygen_fixed.jar cfr.jar fernflower
BurpLoaderKeygen.jar decompiled
BurpLoaderKeygen_modified.jar extracted_original
```
```
hello@hello-friend:~/Desktop/burp2$ java -jar BurpLoaderKeygen_fixed.jar
Success: '/usr/lib/jvm/java-21-openjdk-amd64/bin/java' can execute!
Success: '/usr/lib/jvm/java-21-openjdk-amd64/bin/java' can execute!
```
