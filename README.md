# CTF-ABC
Basic operation of the CTF    
# 常见题型    
* CTF比赛通常包含的题目类型包括MISC、PPC、CRYPTO、PWN、REVERSE、WEB、STEGA。   
* MISC(Miscellaneous)类型，即安全杂项，题目或涉及流量分析、电子取证、人肉搜索、数据分析等等。  
* PPC(Professionally Program Coder)类型，即编程类题目，题目涉及到编程算法，相比ACM较为容易。   
* CRYPTO(Cryptography)类型，即密码学，题目考察各种加解密技术，包括古典加密技术、现代加密技术甚至出题者自创加密技术。  
* PWN类型，PWN在黑客俚语中代表着攻破、取得权限，多为溢出类题目。   
* REVERSE类型，即逆向工程，题目涉及到软件逆向、破解技术。    
* STEGA(Steganography)类型，即隐写术，题目的Flag会隐藏到图片、音频、视频等各类数据载体中供参赛者获取。   
* WEB类型，即题目会涉及到常见的Web漏洞，诸如注入、XSS、文件包含、代码执行等漏洞。  

# 密码类型及解码方法

1.【brainfuck】    
* +++++ +++++ [->++ +++++ +++<] >++.+ +   

* 【解密网站】       https://www.splitbrain.org/services/ook
---
2.【摩斯密码】      
* .-.-.-.-.     

* 【解密】         http://www.atool.org/morse.php
---
3.【键盘坐标密码】   
* 11 21 31 18 27 33 34
* 【手动破解】    
　第二位大于三的是以y为坐标 q是11 a是21 z是31以此类推  
　第二位小于等于三的是以x为坐标 q是11 a是12 w是21 
---
4.【猪圈密码】     
　 ``　------　``    
 　`` |　　　　| ``     
 　`` |　　　　| ``    
 　``　------　``
  
* 【解密】          https://wenku.baidu.com/view/e957c79468dc5022aaea998fcc22bcd126ff4280.html  
---
5.【凯撒密码】     
* VprPGS{jnvg_bar_cyhf_1_vf_3?}   
* 【ctfcracktools】https://github.com/0Chencc/CTFCrackTools/releases/
***

6.【base64】       
* ZmxhZ3tpY3FlZHVfZ29nb2dvX2Jhc2U2NH0
 
* 【解密】         http://tool.oschina.net/encrypt?type=3
***

7.【16进制转字符串】 
* 666c61677b686578327374725f6368616c6c656e67657d 
* 【解密】           https://www.bejson.com/convert/ox2str/
***

8.【栅栏密码】      
* f5-lf5aa9gc9{-8648cbfb4f979c-c2a851d6e5-c}
* 【ctfcracktools】 https://github.com/0Chencc/CTFCrackTools/releases/
***

9.【xxencode】      
* LNalVNrhIO4ZnLqZnLpVsAqtXA4FZTEc+
* 【解密】          http://web.chacuo.net/charsetxxencode/
***

10.【二进制转字符串】  
* 01100110011011000110000101100111011110110110001101100101001100110110010100110101001
* 【解密】            http://www.5ixuexiwang.com/str/from-binary.php   
* 去掉所有的空格放到网站内的转换框
***

11.【quoted 可打印字符编码】     
* =E6=8A=80=E6=9C=AF=E6=9C=89=E6=B8=A9=E5=BA=A6
* 【解密】                  http://www.mxcz.net/tools/QuotedPrintable.aspx
***

12.【培根密码】              
* abbab_babbb_baaaa_aaabb
* 【ctfcracktools】        https://github.com/0Chencc/CTFCrackTools/releases/
***

13.【键盘形状密码】         
* wdvtdz  qsxdr werdzxc  esxcfr uygbn

* 【在键盘上找字母连成的字母】
***
14.【字符频率统计】
* 【解密】 https://quipqiup.com/
---
【图片隐写】            
* 颜色过滤，Stegsolve    
* 隐藏，直接用记事本打开（notepad++更好点） 
* 需要转换成压缩包形式的
* 需要进行Data extract 然后重新保存，利用Stegsolve进行转换提取
* 进行google或者百度搜图
---
【音频隐写】   
* 用Sonic Visualiser 查看图谱 layer add spectrogram/add peak frequency spectrogram
***

# 【【PHP漏洞类型】】


* 【超全局变量GLOBALS漏洞】 当代码中出现类似 $$a 字样时可能存在超全局变量漏洞

* 【MD5 compare漏洞】利用phpMD5不能解析数组的漏洞 构造例如 ?a[]=1&b[]=2 的 payload





 




 
  
