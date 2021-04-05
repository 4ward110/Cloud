# Hiểu về cloud:

- Ảo hóa!!
  - Trừu tượng hóa phần cứng: Compute(CPU, RAM) , Network, Storage
  - Virtualization: ra đời trong những năm 196x trong máy tính mainframes
  -  Hardware/Servẻr/Network/Storage/Desktop/... virtualization
 > Trong lĩnh vực điện toán, thuật ngữ "Virtualization" đề cập đến hành độgn tạo ra phiên bản "Ảo" chứ không phải thực tế của một cái gì đó, bao gồm trong một máy tính ảo với nền tảng phần cứng, hệ đh, thiết bị lưu trữ hoặc cả một tập tài nguyên về mạng máy tính ... nhưng không bị hạn chế.(Thay vì cài một máy lên 1 máy chủ duy nhật => cài qua phần mềm ảo hóa như VMware, KVM,...).
 - Tại sao cần ảo hóa?
   - Giảm cost
   - Tương thích nhiều ứng dụng và điều hành đồng thời
   - Dễ dàng sao lưu và khôi phục
   - Khai thác nhiều hơn về công suất hđ của phần cứng
   - Live migration
   - Là bước đệm lên cloud computing
  - Phân loại các công nghệ ảo hóa: ([Đọc thêm](https://news.cloud365.vn/kvm-tong-quan-ve-virtualization-va-hypervisor/))
    - Full virtual:(Trước khi cài đặt cần lớp OS)
      - Open source: KVM, Virtualbox, KQEMU
      - Thương mại: VMware, Micorsoft(Hyper-V) 
    - Para virtual:(Ko cần OS)
      - Xem, VMWare
    - OS-Level virtual:
      - OpenVZ
      - Linux-VServer
      - Docker      
   ![](https://yoyoclouds.files.wordpress.com/2012/04/2.png)
    - Hosted architecture:
      - Được cài đặt và chạy như một ứng dụng
      - Dựa vào hệ điều hành của máy vật lý để quả lý tài nguyên máy ảo và việc hỗ trợ thiết bị
     - Bare-Metal architecture:
      - Ảo hóa từ "lõi"- trong kernel
      - Cài đặt trực tiếp lên phần cứng.
   - Phần biệt Virtualization và Hypervisor.
    - Hyper: VMware workstation,KVM,ESX => giải quyết bài toán ảo hóa nhằm quản lý máy ảo.Là sp phần mềm để hiện thực hóa Virtualization
    - Virtualization: là 1 khái niệm để tạo 1 hay nhiều máy tính trên cùng 1 đvị phần cứng
- Địng nghĩa Cloud Computing?
  > Định nghĩa từ NIST: Cloud computing is a model for enabling ubiquitous, convenient, on-demand network access to a shared pool of configurable computing resources (e.g., networks, servers, storage, applications, and services) that can be rapidly provisioned and released with minimal management effort or service provider interaction. This cloud model is composed of five essential characteristics, three service models, and four deployment models.   
- Một sản phẩm cloud computing cần có đáp ứng đủ những tiêu chí về: Đặc tính (5), Mô hình triển khai(4), Mo hình dịch vụ(3).
  - 5 Đặc tính của Cloud computing: 
    - On-demand self-service :khả năng tự phục vụ của ng dùng, chủ động khởi tạo, tạm dừng dịch vụ 
    - Broad network access :truy cập trên mọi nền tảng tbi, hạ tầng mạng, khu vực
    - Resource pooling : ng dùng có khả nằng gộp, gom tài nguyên vật lý sau đó phân bổ cho ng dùng tùy theo nhu cầu
    - Rapid elasticity : khả năng "co giãn & đàn hồi" tài nguyên 1 cách nhanh chóng và thuận tiện. có thể cấp phát và thu hồi nhanh chóng
    - Mesured service(pay as you go): đo lường dịch vụ để kiểm soát thời lượng dùng => tính toán phí theo mức độ sử dụng
  - 4 mô hình triển khai:
    - Private cloud:
    - Community Cloud: kết hợp nhiều cloud service provider
    - Public Cloud: cung cấp dịch vụ cho khách hàng sử dụng qua internet như AWS,AZure, GCP, VCCorp, Viettel, NhanHoa
    - Hybrid Cloud: Collab Private & Public
  - 3 mô hình dịch vụ:
  ![](http://researchhubs.com/uploads/cloud-service-models.png) 
   ![](https://www.researchgate.net/profile/Hitesh-Bheda/publication/259865832/figure/fig1/AS:392702911893512@1470639078762/Cloud-Computing-Service-Model.png)
- Ưu / Nhược:
 ![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS4i8qbns5xTaHS1PiqFqccth3H0apGLxMu3RV9t8WFApOv-noI0q7TZNGT2fRqd72al1w&usqp=CAU)
 
   
