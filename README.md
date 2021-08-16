## android openssl 1.0.2

### 准备 下载NDK 编译器 android-ndk-r10e。
### 编译openssl-OpenSSL_1_0_2-stable https://github.com/rocktan001/openssh-portable-V_5_9
### 配置文件generate_standalone_toolchain.sh
#### 注意：配置文件中更改opssl 库目录 。OPENSSL_DIR=/media/disk2/third/android/openssl-OpenSSL_1_0_2-stable/

#### source generate_standalone_toolchain.sh
#### ./configure --host=arm-linux --sysconfdir=${OPENSSH_DIR}/etc/ssh --with-ssl-dir=${OPENSSL_DIR}
#### cp prebuilt-intermediates/config.h ./config.h
### make && make install