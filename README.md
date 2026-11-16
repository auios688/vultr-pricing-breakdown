# Vultr giá rẻ: gói $2.50 có dùng được không, nên chọn $5 hay $6, và một năm thực sự tốn bao nhiêu?

Gói rẻ nhất của Vultr là **$2.50/tháng**, nhưng nó chỉ có IPv6 và 0,5GB RAM. Gói đó đủ để ping thử hoặc chạy một container nhỏ trong lab, không đủ cho một website có người truy cập thật. Phần lớn người đọc nên bắt đầu ở gói **$5/tháng** (1 vCPU, 1GB RAM, 25GB SSD), hoặc **$6/tháng** nếu cần NVMe và CPU đời mới.

Bài dưới đây gồm bảng giá đầy đủ các dòng máy của Vultr, cách tính chi phí thật của một năm (có backup, snapshot, băng thông), và những khoản cộng thêm mà trang đặt hàng không hiển thị ngay.

## Nên chọn gói nào trong 30 giây

> - **Chỉ test IPv6, lab nội bộ, học Linux**: gói $2.50 (1 vCPU · 0,5GB · 10GB SSD · 0,5TB).
> - **Blog, landing page, website ít truy cập, WordPress nhẹ**: gói $5 (1 vCPU · 1GB · 25GB SSD · 1TB).
> - **Cần NVMe, CPU AMD EPYC/Xeon đời mới, single-core nhanh hơn**: gói $6 (1 vCPU · 1GB · 25GB NVMe).
> - **Chạy database, production, không muốn bị hàng xóm lấy mất CPU**: Optimized Cloud Compute từ $28–$30/tháng với vCPU riêng.

👉 [Xem bảng giá và chọn gói Vultr hiện tại](https://www.vultr.com/pricing/?ref=9738262-9J)

## Bảng giá Vultr đầy đủ: Cloud Compute, Optimized, VX1 và GPU

Cloud Compute là dòng dùng chung vCPU, chia làm ba nhóm. Giá dưới đây là giá niêm yết theo tháng, chưa gồm backup và các dịch vụ cộng thêm.

| Gói | Cấu hình | Giá/tháng | Phù hợp với | Đặt gói |
| --- | --- | --- | --- | --- |
| Regular 512MB (IPv6 only) | 1 vCPU · 0,5GB · 10GB SSD · 0,5TB | $2.50 | Test IPv6, lab | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| Regular 512MB (có IPv4) | 1 vCPU · 0,5GB · 10GB SSD · 0,5TB | $3.50 | Test có IPv4 | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| Regular 1GB | 1 vCPU · 1GB · 25GB SSD · 1TB | $5 | Blog, site nhỏ | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| Regular 2GB | 1 vCPU · 2GB · 55GB SSD · 2TB | $10 | Site có cache, vài site | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| Regular 4GB | 2 vCPU · 4GB · 80GB SSD · 3TB | $20 | Web server nhỏ, staging | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| Regular 8GB | 4 vCPU · 8GB · 160GB SSD · 4TB | $40 | Web + app nhỏ | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| Regular 16GB | 6 vCPU · 16GB · 320GB SSD · 5TB | $80 | Nhiều site, traffic vừa | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| Regular 32GB | 8 vCPU · 32GB · 640GB SSD · 6TB | $160 | Ứng dụng nặng RAM | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| High Performance 1GB | 1 vCPU · 1GB · 25GB NVMe | $6 | Cần NVMe, CPU mới | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| High Performance 2GB | 1 vCPU · 2GB · 50GB NVMe | $12 | Web app, cache | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| High Performance 4GB | 2 vCPU · 4GB · 100GB NVMe | $24 | API, DB nhỏ | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| High Performance 8GB | 4 vCPU · 8GB · 180GB NVMe | $48 | Production vừa | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| High Performance 16GB | 8 vCPU · 16GB · 350GB NVMe | $96 | Production, traffic cao | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| High Frequency 1GB | 1 vCPU 3GHz+ · 1GB · 32GB NVMe | $6 | Single-thread nhanh | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| High Frequency 2GB | 1 vCPU 3GHz+ · 2GB · 64GB NVMe | $12 | PHP, xử lý tuần tự | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| High Frequency 4GB | 2 vCPU 3GHz+ · 4GB · 128GB NVMe | $24 | Web có tính toán | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| High Frequency 8GB | 3 vCPU 3GHz+ · 8GB · 256GB NVMe | $48 | CI/CD, encode nhẹ | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| High Frequency 16GB | 4 vCPU 3GHz+ · 16GB · 384GB NVMe | $96 | Build, xử lý nặng | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |

Regular dùng CPU Intel thế hệ trước và SSD thường. High Performance dùng AMD EPYC hoặc Intel Xeon mới hơn, ổ NVMe. High Frequency đẩy xung nhịp lên trên 3GHz, hợp với tác vụ chạy một luồng.

Dòng Optimized Cloud Compute cho vCPU riêng, không chia sẻ với người khác. Đây là chỗ giá nhảy lên một bậc:

| Dòng | Cấu hình khởi điểm | Giá từ | Cấu hình cao nhất | Đặt gói |
| --- | --- | --- | --- | --- |
| CPU Optimized | 1 vCPU · 2GB · 25GB NVMe | $28 | 32 vCPU · 64GB · 1000GB ($720) | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| General Purpose | 1 vCPU · 4GB · 30GB NVMe | $30 | 96 vCPU · 256GB · 1280GB ($3.840) | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| Memory Optimized | 1 vCPU · 8GB · 50GB NVMe | $40 | 32 vCPU · 256GB · 3200GB ($1.565) | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| Storage Optimized | 1 vCPU · 8GB · 150GB NVMe | $75 | 32 vCPU · 256GB · 5760GB ($2.000) | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| VX1 2C/8G/50GB | 2 vCPU · 8GB · 50GB | $48.80 | — | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| VX1 2C/8G/120GB | 2 vCPU · 8GB · 120GB | $55.48 | — | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |
| VX1 4C/16G/240GB | 4 vCPU · 16GB · 240GB | $110.16 | — | [ Xem giá](https://www.vultr.com/pricing/?ref=9738262-9J) |

GPU tính theo giờ, không tính theo tháng:

| GPU | Cấu hình | Giá/giờ |
| --- | --- | --- |
| NVIDIA HGX H100 | 8× H100, 640GB GPU RAM, 224 vCPU | $23.92 |
| NVIDIA L40S | 1 / 2 / 4 / 8 GPU | $1.67 / $3.34 / $6.68 / $13.37 |
| NVIDIA A40 | 1 / 4 GPU | $1.71 / $6.85 |
| AMD MI355X | 8 GPU (preemptible) | $20.72 |

## Gói $2.50 có dùng được không?

Với phần lớn người đọc: không. Gói này chỉ gắn địa chỉ IPv6, không có IPv4. Bạn chỉ truy cập được nếu thiết bị và mạng của bạn hỗ trợ IPv6; nhiều mạng Wi-Fi, nhiều nhà cung cấp di động và gần như toàn bộ khách truy cập website thông thường sẽ không vào được. Đây là lý do phổ biến nhất khiến người mua gói rẻ nhất rồi thấy server "không kết nối được".

Cấu hình đi kèm cũng rất mỏng: 0,5GB RAM, 10GB ổ. Ubuntu 22.04 tối thiểu đã ăn khoảng 300–500MB RAM khi chạy, chưa tính web server hay database. Cài thêm MySQL hoặc Docker là hết chỗ.

Có một chi tiết ít được nói: theo dữ liệu giá của bên thứ ba kiểm tra ngày 12/11/2026, gói $2.50 và gói $3.50 (bản 512MB có IPv4) chỉ được bán ở một vài datacenter, chủ yếu New Jersey, riêng bản IPv6-only còn có ở Atlanta. Nếu chọn Singapore hay Tokyo mà không thấy gói $2.50 trong danh sách, đó là lý do.

Cần IPv4 thì chọn từ gói $3.50 trở lên. Con số $3.50 xuất hiện trong dữ liệu giá của bên thứ ba; giá hiển thị lúc đăng ký là con số quyết định.

👉 [So sánh gói $2.50, $3.50 và $5 trên trang giá Vultr](https://www.vultr.com/pricing/?ref=9738262-9J)

## Chi phí thật của gói rẻ: những khoản cộng thêm

Giá niêm yết chưa phải số tiền bạn trả. Vultr tính thêm vài thứ mà chỉ khi bật lên mới thấy.

**Backup tự động cộng 20%.** Bật backup cho một instance, phí tháng và phí giờ tăng thêm 20% trên giá gốc. Gói $5 thành $6/tháng. Vultr giữ hai bản backup gần nhất, không phải bản theo ngày tùy chọn.

**Snapshot tính riêng $0.05/GB/tháng.** Một snapshot 20GB là $1/tháng, cộng dồn đến khi bạn xóa.

**Block storage $0.10/GB/tháng**, dung lượng tối thiểu 10GB. **Object storage** bản Standard $0.018/GB/tháng, tối thiểu 250GB, kèm 1TB băng thông.

**Băng thông vượt mức $0.01/GB.** Mỗi instance có hạn mức miễn phí, ví dụ gói 2 vCPU/4GB là 3TB/tháng, các gói nhỏ hơn thấp hơn. Vượt quá thì trả $0.01/GB, và cách tính là lấy **mức cao hơn giữa lưu lượng vào và ra**, không cộng hai chiều lại.

**DDoS protection không nằm trong gói**, muốn bật thì thêm $10/tháng, giới hạn 10Gbps.

**Không có chế độ tạm dừng giữ nguyên ổ và IP.** Vultr không hỗ trợ shelving. Muốn ngừng trả tiền thì phải xóa instance; dựng lại từ snapshot hoặc backup nếu cần giữ dữ liệu.

Một phép tính cho gói phổ biến nhất: $5/tháng + backup 20% = $6/tháng, tức **$72/năm**. Thêm một snapshot 20GB ($1/tháng) là $84/năm. Con số này vẫn thấp, nhưng nếu bạn so sánh với bảng giá $5 thì nên biết trước.

👉 [Xem giá gói $5 và các tùy chọn backup trên trang Vultr](https://www.vultr.com/pricing/?ref=9738262-9J)

## Trả theo giờ: $20 dùng được bao lâu?

Vultr tính theo giờ và trừ dần, xóa instance là dừng tính tiền. Quy đổi từ giá tháng (730 giờ): gói $5 khoảng $0.007/giờ, gói $6 khoảng $0.008/giờ, gói $2.50 khoảng $0.0034/giờ. Với $20 trong tài khoản:

- Gói $2.50: khoảng 8 tháng nếu chạy liên tục.
- Gói $5: khoảng 4 tháng.
- Gói $6: khoảng 3 tháng rưỡi.
- Gói $12: khoảng 1 tháng rưỡi.

Cách tiết kiệm thực tế là tạo nhiều máy trong thời gian ngắn rồi xóa. Năm máy test chạy hai giờ mỗi máy, gói $6, tốn chưa tới $0.10. Thời gian khởi tạo trung bình khoảng 77 giây theo 12 lần đo của vpsbenchmarks, nhanh nhất 30 giây, chậm nhất hơn 4 phút.

Có một giới hạn cần biết trước khi định chạy nặng trên gói rẻ: Vultr giới hạn instance dùng chung vCPU nếu nó chiếm CPU, ổ đĩa hoặc băng thông ở mức ảnh hưởng người khác. Trên Trustpilot có phản ánh server bị tạm ngưng vì lý do tài nguyên. Khi đó cách xử lý là chuyển sang Optimized Cloud Compute hoặc Bare Metal, không phải mở ticket xin bỏ giới hạn.

## Mã giảm giá Vultr: $300, $250 hay hoàn tiền 100%?

Trang coupons chính thức của Vultr đang niêm yết bốn chương trình cho tài khoản mới, và chúng khác nhau ở thời hạn chứ không chỉ ở con số.

| Chương trình | Giá trị | Thời hạn | Điều kiện đáng chú ý |
| --- | --- | --- | --- |
| FLY300VULTR | $300 credit | 30 ngày | Cần liên kết thẻ tín dụng hoặc PayPal; phần chưa dùng hết sau 30 ngày bị mất |
| FLYTWOHUNDRED | $200 credit | 30 ngày | Tài khoản mới |
| 250VULTRFLY | $250 credit | 30 ngày | Tài khoản mới |
| VULTRMATCH | Hoàn tiền 1:1, tối đa $100 | 12 tháng | Nạp trước, Vultr cộng thêm đúng số đã nạp |

VULTRMATCH có một cơ chế ít người để ý: credit được trừ theo tỷ lệ 50/50. Nếu số dư phát sinh trong giờ là $10, $5 lấy từ credit khuyến mãi và $5 lấy từ tiền thật bạn nạp. Nghĩa là tiền thật của bạn vẫn bị dùng song song, không phải credit gánh hết trước.

Chọn thế nào: nếu bạn định dựng thử nhiều cấu hình, benchmark GPU, hoặc test vài datacenter trong vài tuần, chọn gói 30 ngày. Nếu bạn định giữ một VPS $5–$6 chạy blog dài hạn, VULTRMATCH thực dụng hơn vì credit sống 12 tháng. Mã có thể thay đổi theo thời điểm, nên xem ô nhập mã ở bước thanh toán để biết mã nào còn hiệu lực.

👉 [Đăng ký Vultr và kiểm tra mã credit đang áp dụng](https://bit.ly/VuLtr)

## Vultr so với DigitalOcean và Linode ở điểm nào?

Cả ba đều tính theo giờ và đều nhắm vào nhóm người dùng không muốn trả trước nhiều tháng. Khác biệt đáng kể nhất với người ở Việt Nam nằm ở vị trí datacenter: Vultr không có datacenter tại Việt Nam, gần nhất là Singapore và Tokyo, cộng thêm Osaka, Seoul, Mumbai, Bangalore và Delhi NCR trong danh sách châu Á. DigitalOcean và Linode có ít lựa chọn hơn ở khu vực này, nhưng bài viết không so sánh giá của họ vì bảng giá của họ thay đổi và chưa được kiểm tra lại trong lần rà soát này.

Về số lượng datacenter, thống kê ngày 01/11/2026 của vpsbenchmarks ghi nhận Vultr có 31 datacenter trên 5 châu lục. Cùng một cấu hình được bán với giá như nhau ở hầu hết địa điểm, ngoại lệ là São Paulo tính 1,5 lần giá niêm yết.

## Câu hỏi thường gặp

**Gói $2.50 có IPv4 không?**
Không. Gói này chỉ có IPv6. Muốn có IPv4 thì chọn gói cao hơn một bậc.

**Nhận $300 credit mà 30 ngày không dùng hết thì sao?**
Phần chưa dùng bị mất sau 30 ngày. Credit cũng cần tài khoản đã liên kết thẻ tín dụng hoặc PayPal hợp lệ.

**Bật backup có mất thêm tiền không?**
Có. Phí tháng và phí giờ tăng 20% trên giá gốc của instance.

**Có tạm dừng server để tiết kiệm không?**
Vultr không có tính năng shelving. Muốn dừng tính tiền thì phải xóa instance.

**VPS bị suspend là do đâu?**
Thường là do dùng quá nhiều tài nguyên trên instance dùng chung vCPU, ảnh hưởng đến người khác. Cách xử lý là chuyển sang dòng Optimized hoặc Bare Metal.

**Support của Vultr có tệ không?**
Điểm đánh giá rất chênh lệch: HostAdvice 2,2/5, Trustpilot 1,7/5, trong khi G2 khoảng 4,3/5. Nhóm phàn nàn chủ yếu là người dùng cá nhân gặp sự cố cần hỗ trợ nhanh; nhóm đánh giá cao thường là developer quen tự xử lý.

## Chọn theo tình huống

Chỉ cần một máy IPv6 để học hoặc test nội bộ: gói $2.50, chấp nhận việc không truy cập được từ mạng IPv4. Blog, portfolio, landing page ít traffic: gói $5, thêm backup nếu có dữ liệu người dùng. Cần NVMe và CPU đời mới cho cùng số tiền: gói $6 của High Performance hoặc High Frequency. Chạy database, API production hoặc bất cứ thứ gì không được phép bị hàng xóm giành CPU: Optimized Cloud Compute, khởi điểm $28 với CPU Optimized.

Trước khi bấm tạo server, xác nhận hai việc: bạn có định dùng credit khuyến mãi không (nếu có, phải liên kết thẻ hoặc PayPal và biết hạn 30 ngày hay 12 tháng), và bạn có định bật backup không (cộng 20% vào hóa đơn tháng). Chọn sai datacenter cũng là lỗi hay gặp: không có node Việt Nam, nên chọn Singapore hoặc Tokyo nếu người dùng chính ở Đông Nam Á.

👉 [Chọn gói Vultr phù hợp và tạo server trong vài phút](https://www.vultr.com/pricing/?ref=9738262-9J)
