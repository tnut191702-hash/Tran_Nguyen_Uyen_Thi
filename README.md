# DỰ ÁN: NGUYÊN LÍ DIRICHLET VÀ MỘT SỐ ỨNG DỤNG TRONG THỰC TIỄN

> Dự án **Nguyên lí Dirichlet và một số ứng dụng trong thực tiễn**, được biên soạn và trình bày chuyên nghiệp bằng LaTeX.  Báo cáo nghiên cứu ứng dụng Toán học Tổ hợp trong Khoa học Máy tính, Y sinh, Quy hoạch Hạ tầng và Mạng Xã hội.

---
## Giới Thiệu 

Nguyên lý Dirichlet (hay còn gọi là *Nguyên lý Lồng chim / Chuồng thỏ* – *Pigeonhole Principle*) được phát biểu bởi nhà toán học người Đức **Johann Peter Gustav Lejeune Dirichlet** (1805–1859). 

Dù mang ý tưởng thực tiễn đơn giản: *"Nếu nhốt n+1 con thỏ vào n cái chuồng thì chắc chắn có ít nhất một chuồng chứa từ 2 con thỏ trở lên"*, nguyên lý này là một công cụ suy luận phản chứng cực kỳ mạnh mẽ. Điểm mấu chốt nằm ở kỹ năng **thiết lập ánh xạ phân loại ("Thỏ" và "Chuồng")** để chuyển hóa các bài toán thực tế phức tạp về dạng đánh giá sự trùng lặp hoặc ngưỡng bùng phát của hệ thống.

---

## 📖 1. Nội Dung Chính Trong Báo Cáo

### A. Giới Thiệu Chung
* **Lý do chọn đề tài:** Khai thác tư duy phân loại đối tượng ("Thỏ" và "Chuồng") để giải quyết các bài toán thực tế như trùng lặp dữ liệu, tối ưu bộ nhớ, phân luồng giao thông.
* **Mục đích & Nhiệm vụ:** Hệ thống hóa các dạng phát biểu, phân tích ứng dụng trong CNTT, Giao thông, Logistics, Sinh học và giải bài toán minh họa.
* **Đối tượng & Phạm vi:** Cơ sở lý luận nguyên lý Dirichlet và quy trình mô hình hóa toán học thiết lập ánh xạ.

### B. Cơ Sở Lý Thuyết
Hệ thống hóa các dạng phát biểu toán học và quy trình mô hình hóa :
* **Nguyên lý Dirichlet cơ bản:** Nhốt $n+1$ con thỏ vào $n$ chuồng.
* **Nguyên lý Dirichlet tổng quát:** Phân bố $n$ đồ vật vào $k$ hộp $\Rightarrow$ Tồn tại hộp chứa ít nhất $\lceil n/k \rceil$ đồ vật.
* **Nguyên lý Dirichlet mở rộng:** Dùng hàm sàn $\lfloor \cdot \rfloor$ đánh giá ngưỡng $\lfloor (n+m-1)/m \rfloor$.
* **Nguyên lý Dirichlet dạng tập hợp:** Khảo sát ánh xạ $f: A \to B$ khi $|A| > |B|$, chứng minh $f$ không thể là đơn ánh.
* **Nguyên lý Dirichlet trong hình học liên tục:** Áp dụng cho vùng không gian có độ đo và đường kính giới hạn $d$.

### C. Các Lĩnh Vực Ứng Dụng Thực Tế
* **Khoa học Máy tính & An ninh mạng:**
  * **Va chạm mã băm (Hash Collisions):** Khảo sát miền xác định vô hạn $\aleph_0$ và miền giá trị $2^n$ bits.
  * **Nén dữ liệu không mất thông tin (Lossless Data Compression):** Chứng minh tính vô lý của thuật toán nén mọi tệp tin đầu vào.
  * **Mã kiểm tra & Mã sửa lỗi (Checksum & CRC):** Chứng minh sự tồn tại của "điểm mù" (undetectable errors) trong truyền nhận gói tin.
* **Phân tích Gen & Y sinh:**
  * Xác định điều kiện độ dài chuỗi DNA ($N \ge 4^k + k$) để bắt buộc xuất hiện các đoạn $k$-mer lặp lại, phục vụ định danh loài và phát hiện bệnh di truyền.
* **Quy hoạch Hạ tầng & Cân bằng tải:**
  * **Cân bằng tải Máy chủ (Server Load Balancing):** Xác định số lượng máy chủ tối thiểu $M \ge \lceil N/C \rceil$ để tránh quá tải.
  * **Mật độ Lưu lượng Giao thông:** Xác định điểm bùng phát ùn tắc làm cơ sở xây dựng thuật toán điều khiển đèn giao thông thích ứng.
* **Lý thuyết Đồ thị & Mạng Xã hội:**
  * Chứng minh trong đồ thị $n$ đỉnh luôn tồn tại ít nhất 2 đỉnh có cùng bậc (mỗi mạng xã hội luôn có 2 người có cùng số bạn).
  * **Định lý Ramsey $R(3,3)=6$:** Tìm bộ ba quen biết/không quen biết trong nhóm 6 người.

### D. Bài Toán Thực Tế Minh Họa
1. **Thương mại điện tử:** Đánh giá rủi ro nghẽn hệ thống khi 8 máy chủ tiếp nhận 12.500 lượt truy cập/phút.
2. **Sinh học:** Chứng minh sự lặp lại của đoạn 4-mer trong chuỗi DNA 1.000 nucleotide.
3. **Quản trị nhân sự:** Đánh giá tính khả thi trong lịch phân công ca trực cấp cứu của 30 bác sĩ.
4. **Mạng xã hội:** Áp dụng Định lý Turán/Mantel chứng minh sự tồn tại của "Bộ ba siêu kết nối" trong mạng 20 tài khoản có 101 kết nối.

---

## 📚 2. Tài Liệu Tham Khảo

1. **Nguyễn Hữu Điển (1999)**, *Phương pháp Dirichlet và ứng dụng*, NXB Khoa học và Kỹ thuật Hà Nội.
2. **Kenneth H. Rosen (2019)**, *Discrete Mathematics and Its Applications*, 8th Edition, McGraw-Hill Education.
3. **Cormen, T. H., Leiserson, C. E., Rivest, R. L., & Stein, C. (2009)**, *Introduction to Algorithms*, 3rd Edition, MIT Press.
4. **Dar, Z. S. (2018)**, *The Pigeonhole Principle and It's Applications*, Undergraduate Seminar, Jacobs University Bremen.
