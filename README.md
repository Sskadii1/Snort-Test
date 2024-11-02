# Snort-Test
snort

Cài đặt các gói phụ thuộc: Snort cần một số gói phụ thuộc để hoạt động. Bạn có thể cài đặt chúng bằng lệnh:

![image](https://github.com/user-attachments/assets/fc94cadf-6f81-4e91-8ea7-64ef1fb773d9)
Cài đặt DAQ:
wget https://www.snort.org/downloads/archive/snort/daq-2.0.7.tar.gz

Cài đặt SNORT ver 2.9.21:
wget https://www.snort.org/downloads/snort/snort-2.9.21.tar.gz

![image](https://github.com/user-attachments/assets/b97bb9e0-bea0-4d11-8555-18e1bc0f2110)

Giải nén tệp

![image](https://github.com/user-attachments/assets/d0a997f3-9bc8-4b6b-b5e7-93380fbff9ff)



![image](https://github.com/user-attachments/assets/41762276-ad74-4afb-bf22-2ee708d2adee)

config
![image](https://github.com/user-attachments/assets/7283d43d-437e-4167-94a8-f5294182afc2)
 tải snort thành công
![image](https://github.com/user-attachments/assets/8807c7c3-597e-4ece-bdd9-7631bc89b16f)

Snort có một số tệp quy tắc tích hợp, tệp cấu hình và các tệp khác. Những tệp này được lưu trữ trong /etc/snortthư mục.
![image](https://github.com/user-attachments/assets/e05634f4-b00e-42e1-af3f-3d9fb5500a66)

Tệp chính của Snort là tệp cấu hình snort.conf, nơi bạn có thể chỉ định tệp quy tắc nào sẽ được bật và phạm vi mạng nào sẽ được giám sát và bật các cài đặt khác. Các tệp quy tắc được lưu trữ trong rulesthư mục. Hãy sử dụng lslệnh để liệt kê tất cả các tệp và thư mục có trong thư mục chính của Snort

**Định dạng quy tắc**

Bây giờ, chúng ta hãy thảo luận về cách tạo quy tắc trong Snort. 

Sau đây là một quy tắc mẫu sẽ phát hiện các gói tin ICMP (thường được sử dụng khi bạn ping một máy chủ) đến từ bất kỳ địa chỉ IP và cổng nào và đến mạng gia đình (phạm vi mạng được xác định trong tệp cấu hình của Snort) đến bất kỳ cổng nào. Khi phát hiện lưu lượng truy cập như vậy, nó sẽ tạo cảnh báo "Ping Detected".

![image](https://github.com/user-attachments/assets/b90f3131-f0c9-435e-9580-58ea8e11ee56)
**nguồn tryhackme**


Sau khi cài đặt, chúng ta có thể chạy Snort, và để nó lưu lại lưu lượng dành cho máy chủ của bạn, tùy nhiên, để mà snort có thể ghi lại và phát hiện xâm nhập mạng của bạn, thì phải bật chế độ promiscuous mode, của máy chủ mạng của bạn.

**https://thangletoan.wordpress.com/2019/04/02/che-do-promiscuous-dung-o-mang-ao-vmware/*

**https://docs.vmware.com/en/VMware-vSphere/7.0/com.vmware.vsphere.security.doc/GUID-92F3AB1F-B4C5-4F25-A010-8820D7250350.html*

đây là 2 trang về ví dự thực hành, và định nghĩa về chế độ promiscuous mode.






