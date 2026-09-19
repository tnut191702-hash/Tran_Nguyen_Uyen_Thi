# Kế hoạch biên soạn: Khoa học về cơ thể người

## Định dạng kỹ thuật

Dự án được biên soạn bằng **Latex** thay vì Typst/Word, vì:

-   Là chuẩn mực toàn cầu trong xuất bản Toán học, xử lý hoàn hảo các công thức.
-   Tích hợp BibTeX giúp tự động hóa trích dẫn (\cite{...}) và lập danh mục tài liệu tham khảo chính xác.
-   Tách biệt nội dung với giao diện, không bị lỗi nhảy trang hay tràn lề như Word khi tài liệu dài.
-   File .tex là văn bản thuần, dễ chia nhỏ chương, quản lý phiên bản qua Git và theo dõi lịch sử sửa đổi rõ ràng.
## 🛠️ 1. Cấu Trúc Thư Mục & Quy Ước Soạn Thảo

Dự án được triển khai cấp tốc bằng **LaTeX / XeLaTeX** để tối ưu hóa việc dàn trang và quản lý công thức toán học.

### Cấu Trúc Thư Mục Kho Lưu Trữ (Repository)
```text
Dirichlet_Project/
├── docs/
│   ├── Bao_Cao_Dirichlet_UyenThi.pdf   # File PDF xuất bản chính thức (~21 trang)
│   ├── main.tex                        # File LaTeX gốc gom toàn bộ các chương
│   └── chapters/                       # Các file chương độc lập
│       ├── 01_gioi_thieu.tex
│       ├── 02_co_so_ly_thuyet.tex
│       ├── 03_ung_dung_thuc_tien.tex
│       ├── 04_bai_toan_minh_hoa.tex
│       └── 05_ket_luan.tex
├── figures/                            # Hình ảnh & Đồ thị minh họa
│   ├── hash_collision.png
│   ├── dna_kmer.png
│   └── ramsey_graph.png
├── references/
│   └── references.bib                  # Thư viện tài liệu tham khảo BibTeX
├── README.md                           # Giới thiệu tổng quan dự án
└── PLAN.md                             # Lộ trình cấp tốc 2 tuần
```

## 📈 2. Kế Hoạch & Tiến Độ Thực Hiện

- [ ] **Tuần 1:** Hoàn thành Lý thuyết + Mẫu ứng dụng (Ngày 1 - 7)
- [ ] **Tuần 2:** Bài toán thực tế + Biên tập LaTeX & Xuất file PDF (Ngày 8 - 14)
## 🗓️ Lộ Trình
### TUẦN 1: Dựng Khung, Cơ Sở Lý Thuyết & Mô Hình Ứng Dụng (Ngày 1 – Ngày 7)

* **Ngày 1 – 2 (Khởi tạo & Phần Mở đầu):**
  - Khai tạo thư mục dự án, mẫu trang bìa ĐH Sư phạm - ĐH Huế và cấu trúc file LaTeX.
  - Viết xong **Phần Mở đầu**: Lý do chọn đề tài, mục đích, nhiệm vụ, đối tượng và phạm vi nghiên cứu.
* **Ngày 3 – 4 (Cơ sở Lý thuyết Toán học):**
  - Soạn thảo 5 dạng phát biểu: Cơ bản, Tổng quát ($\lceil n/k \rceil$), Mở rộng ($\lfloor \cdot \rfloor$), Dạng tập hợp và Hình học liên tục.
  - Chứng minh các định lý trọng tâm bằng phương pháp phản chứng.
* **Ngày 5 – 7 (Ứng dụng Thực tế Chuyên sâu):**
  - Soạn thảo phần ứng dụng trong **Khoa học Máy tính & An ninh mạng** (Va chạm mã băm, Lossless Compression, CRC).
  - Soạn thảo phần ứng dụng trong **Phân tích Gen Y sinh** (Tìm đoạn k-mer lặp trong DNA).
  - Soạn thảo phần ứng dụng trong **Hạ tầng & Mạng xã hội** (Server Load Balancing, Đồ thị $n$ đỉnh, Định lý Ramsey R(3,3).

---

### TUẦN 2: Bài Toán Minh Họa, Kết Luận & Hoàn Thiện LaTeX (Ngày 8 – Ngày 14)

* **Ngày 8 – 10 (Xây dựng Bài toán Minh họa & Lời giải):**
  - Giải chi tiết **Bài toán 1**: Đánh giá quá tải hệ thống E-commerce (12.500 req/phút / 8 servers).
  - Giải chi tiết **Bài toán 2**: Phân tích sự lặp lại đoạn 4-mer trong chuỗi 1.000 nucleotide DNA.
  - Giải chi tiết **Bài toán 3**: Lịch phân công ca trực cấp cứu cho 30 bác sĩ trong 7 ngày.
  - Giải chi tiết **Bài toán 4**: Ứng dụng Định lý Turán chứng minh "Bộ ba siêu kết nối" trong mạng xã hội.
* **Ngày 11 – 12 (Tổng kết & Trích dẫn):**
  - Viết phần **Kết luận & Hướng phát triển của đề tài**.
  - Chuẩn hóa danh mục 4 Tài liệu tham khảo chuẩn bằng BibTeX (`references.bib`).
* **Ngày 13 – 14 (Chế bản LaTeX, Soát lỗi & Xuất bản PDF):**
  - Vẽ và chèn các sơ đồ đồ thị/hình ảnh minh họa vào báo cáo.
  - Rà soát lỗi chính tả, căn chỉnh lề, định dạng công thức toán học.
  - Biên dịch file PDF hoàn chỉnh (~21 trang) và bàn giao báo cáo.

---

## 📊 3. Bảng Theo Dõi Tiến Độ Theo Ngày

| Ngày | Nội Dung Công Việc | Đầu Ra Dự Kiến | Trạng Thái |
| :---: | :--- | :--- | :---: |
| **N1 - N2** | Tạo khung LaTeX + Viết Phần Mở đầu | File `01_gioi_thieu.tex` | Hoàn thành |
| **N3 - N4** | Viết 5 dạng phát biểu Cơ sở lý thuyết | File `02_co_so_ly_thuyet.tex` | Hoàn thành |
| **N5 - N7** | Viết 4 Lĩnh vực Ứng dụng thực tế | File `03_ung_dung_thuc_tien.tex` | Hoàn thành |
| **N8 - N10** | Giải 4 Bài toán minh họa thực tế | File `04_bai_toan_minh_hoa.tex` | Hoàn thành |
| **N11 - N12** | Viết Kết luận & Chuẩn hóa BibTeX | File `05_ket_luan.tex` + `references.bib` | Hoàn thành |
| **N13 - N14** | Chỉnh LaTeX, vẽ hình & Export PDF chính thức | File `Bao_Cao_Dirichlet_UyenThi.pdf` (~21 trang) | Hoàn thành |

---

## ⚠️ 4. Nguyên Tắc Thực Hiện Cấp Tốc

1. **Tập trung vào tính chuẩn xác của mô hình:** Mọi bài toán ứng dụng bắt buộc phải định nghĩa rõ ràng ngay từ đầu: Tập nguồn $A$ ("Thỏ"), Tập đích $B$ ("Chuồng") và Ánh xạ $f: A \to B$.
2. **Biên dịch LaTeX liên tục:** Biên dịch file sau mỗi ngày làm việc để phát hiện và xử lý ngay các lỗi cú pháp công thức toán.
