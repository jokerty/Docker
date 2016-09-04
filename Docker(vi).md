#DOCKER
###MỤC LỤC
[I. Mở đầu](#modau)


[II. Cài đặt Docker](#caidatdocker)

- [2.1. Docker for Linux](#dockerforlinux)
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

## II. Cài đặt
###2.1. Docker for Linux

###2.2. Docker for Windows