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

**Docker bao gồm:**

- `Docker Engine`: Chứa các tool, engine để có thể đóng gói chương trình và vận hành chúng một cách đơn giản nhất.
- `Docker Hub`: Giống như Github, là nơi bạn có thể lưu trữ các chương trình đã được đóng gói (image) của mình và quản lý các image.

**Vậy lợi ích của Docker là gì?** 

- Một ví dụ đơn giản là chúng ta sử dụng image của ubuntu 12.04 (có sẵn trên Docker Hub). Cài vào image đó ruby on rails, đóng gói và chúng ta đã có 1 bản ubuntu chứa ruby on rails mà có thể lấy và sử dụng ở bất cứ đâu. 
- Hoặc một ví dụ trong Ruby on rail, việc deploy app sẽ trở nên dễ dàng hơn. Không còn những câu lệnh để deploy mà thay vào đó chỉ cần upload image của app lên server rồi sau đó chạy image là xong. 
- Ngoài ra còn có Docker Hub cho phép quản lý các image với những câu lệnh giống như Github như push, pull... để bạn có thể quản lý dễ dàng image của mình. Docker Hub có số lượng image cực kì đa dạng từ các OS như Ubuntu, CentOS... đến các phiên bản Ruby, các phiên bản Rails... để bạn có thể tùy chỉnh các phiên bản này.

<a name="caidatdocker"></a>
## II. Cài đặt Docker

<a name="dockerforlinux"></a>
###2.1. Docker for Linux
[2.1.1. CentOS](#211centOS)

[2.1.2. Ubuntu](#212ubuntu)

[2.1.3. Debian](#213debian)

<a name="211centOS"></a>
- **2.1.1. CentOS**
<ul>
    <li>**Yêu cầu:**</li>

    **Docker yêu cầu 64bit và Kernel version 3.10 trở lên đối với các phiên bản CentOS (nói cách khác là CentOS7.x trở lên)**
    
    Kiểm tra kernel version
    
        $ uname -r
    Trả về:
    
        3.10.0-229.el7.x86_64
    
    <li>**Cài đặt:**</li>
    
    **Cài đặt bằng yum:**

    1. Truy cập vào máy của bạn với quyền root và tiến hành update
    
        `$ sudo yum update`
    2. Tạo 1 yum repo.
    
        ```sh
        $ sudo tee /etc/yum.repos.d/docker.repo <<-'EOF'
        [dockerrepo]
        name=Docker Repository
        baseurl=https://yum.dockerproject.org/repo/main/centos/7/
        enabled=1
        gpgcheck=1
        gpgkey=https://yum.dockerproject.org/gpg
        EOF
        ```

    3. Cài đặt Docker package.
    
        `$ sudo yum install docker-engine`
    4. Chạy Docker daemon.

        `$ sudo service docker start`
    5. Kiểm tra Docker đã được cài đặt và chạy thử demo.

        ```sh
        $ sudo docker run hello-world
        Unable to find image 'hello-world:latest' locally
        latest: Pulling from hello-world
        a8219747be10: Pull complete
        91c95931e552: Already exists
        hello-world:latest: The image you are pulling has been verified. Important: image verification is a tech preview feature and should not be relied on to provide security.
        Digest: sha256:aa03e5d0d5553b4c3473e89c8619cf79df368babd1.7.1cf5daeb82aab55838d
        Status: Downloaded newer image for hello-world:latest
        Hello from Docker.
        ```
    
    Nếu hiển thị ra kết quả như trên thì Docker đã được cài đặt thành công và đang hoạt động.

    **Cài đặt bằng script(curl):**
    
    1. Truy cập vào máy của bạn với quyền root và tiến hành update
    
        `$ sudo yum update`
    2. Chạy cài đặt Docker bằng script.

        `$ curl -fsSL https://get.docker.com/ | sh`
        
        Câu lệnh script sẽ thêm file `docker.repo` và cài đặt Docker.
    
    3. Chạy Docker daemon.

        `$ sudo service docker start`
    4. Kiểm tra Docker đã được cài đặt và chạy thử demo.

        `$ sudo docker run hello-world`
</ul>

<a name="212ubuntu"></a>
- **2.1.2. Ubuntu**
<ul>
<li>**Yêu cầu:**</li>
**Docker yêu cầu 64bit và Kernel version 3.10 trở lên đối với các phiên bản CentOS (nói cách khác là CentOS7.x trở lên)**
    
    Kiểm tra kernel version
    
        $ uname -r
    Trả về:
    
        3.10.0-229.el7.x86_64
    
<li>**Cài đặt:**</li>


</ul>
<a name="dockerforwindows"></a>
###2.2. Docker for Windows
