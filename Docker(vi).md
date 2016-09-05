#DOCKER
###MỤC LỤC
[I. Mở đầu](#modau)


[II. Cài đặt Docker](#caidatdocker)

- [2.1. Docker for Linux](#dockerforlinux)
<ul>
<li>		[2.1.1. CentOS](#211centOS)</li>
<li>		[2.1.2. Ubuntu](#212ubuntu)</li>
<li>		[2.1.3. Debian](#213debian)</li>
</ul>
- [2.2. Docker for Windows](#dockerforwindows) 

<a name="modau"></a>
## I. Mở đầu

####Docker là một open platform cung cấp cho người sử dụng những công cụ và service để người sử dụng có thể đóng gói và chạy chương trình của mình trên các môi trường khác nhau một cách nhanh nhất. 

Docker bao gồm:

- `Docker Engine`: Chứa các tool, engine để có thể đóng gói chương trình và vận hành chúng một cách đơn giản nhất.
- `Docker Hub`: Giống như Github, là nơi bạn có thể lưu trữ các chương trình đã được đóng gói (image) của mình và quản lý các image.

Vậy lợi ích của Docker là gì? 

- Một ví dụ đơn giản là chúng ta sử dụng image của ubuntu 12.04 (có sẵn trên Docker Hub). Cài vào image đó ruby on rails, đóng gói và chúng ta đã có 1 bản ubuntu chứa ruby on rails mà có thể lấy và sử dụng ở bất cứ đâu. 
- Hoặc một ví dụ trong Ruby on rail, việc deploy app sẽ trở nên dễ dàng hơn. Không còn những câu lệnh để deploy mà thay vào đó chỉ cần upload image của app lên server rồi sau đó chạy image là xong. 
- Ngoài ra còn có Docker Hub cho phép quản lý các image với những câu lệnh giống như Github như push, pull... để bạn có thể quản lý dễ dàng image của mình. Docker Hub có số lượng image cực kì đa dạng từ các OS như Ubuntu, CentOS... đến các phiên bản Ruby, các phiên bản Rails... để bạn có thể tùy chỉnh các phiên bản này.

<a name="caidatdocker"></a>
## II. Cài đặt Docker

<a name="dockerforlinux"></a>
###2.1. Docker for Linux

<a name="211centOS"></a>
- **2.1.1. CentOS**
<ul>
<li>**Yêu cầu:**</li>
Docker yêu cầu 64bit và Kernel version 3.10 trở lên đối với các phiên bản CentOS (nói cách khác là CentOS7.x trở lên) 
<li>**Cài đặt:**</li>
Kiểm tra kernel version
    $ uname -r

Trả về:
    3.10.0-229.el7.x86_64

Tiến hành cài đặt:

- Cài đặt bằng yum:
<ul>
<li></li>
<li></li>
</ul>


- Cài đặt bằng yum:
<ul>
<li></li>
<li></li>
</ul>

Gỡ cài đặt
</ul>

<a name="212ubuntu"></a>
- **2.1.2. Ubuntu**
<ul>
<li>**Yêu cầu:**</li>
Chỉ hỗ trợ các phiên bản centos7.x trở lên và các 
<li>**Cài đặt:**</li>
</ul>

<a name="213debian"></a>
- **2.1.3. Debian**
<ul>
<li>**Yêu cầu:**</li>
Chỉ hỗ trợ các phiên bản centos7.x trở lên và các 
<li>**Cài đặt:**</li>
</ul>

<a name="dockerforwindows"></a>
###2.2. Docker for Windows