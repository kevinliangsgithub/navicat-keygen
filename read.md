## 1. 如何编译

  * 在编译之前，你应该确保你安装了OpenSSL。如果你有`brew`的话，你可以通过`brew install openssl`来完成OpenSSL的安装。

    ```bash
    $ cd navicat-keygen
    $ make release
    ```

  * 如果你的Navicat版本号等于或大于12.0.24，你需要编译patcher。

    ```bash
    $ cd navicat-patcher
    $ make release
    ```

## 2. 如何使用这个Keygen

  1. 替换rpk：

       * 用生成或提供的`rpk`文件替换掉`Navicat Premium.app/Contents/Resources/rpk`。

  2. 接下来，打开`Terminal.app`，并定位到`navicat-keygen`文件夹：

     ```bash
     $ ./navicat-keygen 2048key.pem
     ```

     接下来你会被要求输入Navicat的语言版本，然后得到一个 __序列号__，同时keygen会要求你输入用户名和组织名。  
     直接填写，之后你会被要求填写你得到的 __请求码__。注意此时 __不要关闭Terminal__.

  5. 打开Navicat Premium。找到`注册`按钮并点击，在弹出的窗口中填入keygen给你的 __序列号__。然后点击`激活`按钮。

  6. 一般来说在线激活肯定会失败，这时候Navicat会询问你是否`手动激活`，直接选吧。

  7. 在`手动激活`窗口你会得到一个请求码，复制它并把它粘贴到keygen里。最后别忘了连按至少两下回车结束输入。

  8. 如果不出意外，你会得到一个看似用Base64编码的 __激活码__。直接复制它，并把它粘贴到Navicat的`手动激活`窗口，最后点`激活`按钮。如果没什么意外的话应该能成功激活。

  9. 最后，如果你备份了数据库连接配置信息，那么恢复它把。
