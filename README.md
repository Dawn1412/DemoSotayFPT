# sotayFPT_ktv
# 📙 Sổ Tay Kỹ Thuật Viên (KTV) — FPT Telecom

<img width="1920" height="1080" alt="{4FBB53DA-37F6-4CD0-A108-B4D7ACA5A429}" src="https://github.com/user-attachments/assets/15a9238c-9315-44d3-8a82-965c00cafde8" />


![Streamlit](https://img.shields.io/badge/Streamlit-1.30+-FF4B4B?style=for-the-badge&logo=Streamlit&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FPT Telecom](https://img.shields.io/badge/FPT_Telecom-Hue_Branch-F26F21?style=for-the-badge)

Ứng dụng web tra cứu thông minh, hỗ trợ quy trình kỹ thuật, mã lỗi thiết bị và tài liệu chuyên môn dành cho **Kỹ thuật viên hiện trường FPT Telecom Chi nhánh Thừa Thiên Huế**.

---

## 🌟 Tính Năng Nổi Bật

- **🔍 Smart Search (Tìm kiếm thông minh):** Tự động phân tích từ khóa, nhận diện ý định (Intent Recognition) và tự động chuyển Tab/phân hệ hiển thị tương ứng.
- **📂 Quản lý 4 phân hệ cốt lõi:**
  - **Quy trình:** Lắp đặt, bảo trì, xử lý dịch vụ broadband & truyền hình.
  - **Xử lý sự cố:** Tra cứu nhanh danh mục mã lỗi FPT Play, SmartTV, Android, iOS, thiết bị ngoại vi.
  - **Bán hàng:** Cập nhật chính sách, gói cước và chương trình ưu đãi mới nhất.
  - **Tài liệu:** Đào tạo tân binh, tài liệu 4XL, hướng dẫn cấu hình modem/mesh Wi-Fi (AX3000S, Skyworth, Wi-Fi 6...).
- **🌙 Chế độ nền tối (Dark Mode):** Tùy biến giao diện giảm mỏi mắt, hỗ trợ KTV tác nghiệp ứng cứu thông tin vào ca đêm.
- **⚡ Hot-Reload Data:** Tự động đồng bộ và nạp dữ liệu mới nhất từ file Excel gốc mà không làm gián đoạn trải nghiệm người dùng.

---

## 🏗️ Kiến Trúc Hệ Thống & Cấu Trúc Thư Mục

```text
SOTAY_FPT/
├── .streamlit/          # Cấu hình giao diện Streamlit Cloud
├── tailieu/             # Kho tài liệu đính kèm (PDF, Excel, Ảnh sơ đồ)
│   ├── cau_hinh/        # Tài liệu cấu hình thiết bị
│   ├── xu_ly_su_co/     # Sơ đồ và file mã lỗi FPT Play
│   └── 4xl/             # Chương trình chuẩn giao tiếp KTV
├── utils/               # Các hàm tiện ích bổ trợ
├── views/               # Các module giao diện phân hệ
│   ├── quy_trinh.py     # Giao diện Quy trình & Xử lý sự cố
│   ├── ban_hang.py      # Giao diện Phân hệ Bán hàng
│   └── tai_lieu.py      # Giao diện Phân hệ Tài liệu & Tân binh
├── app.py               # Entry point (luồng chính của ứng dụng)
├── data_loader.py       # Module đọc & xử lý cache dữ liệu Excel
├── styles.py            # Custom CSS & Theme Toggle (Dark/Light mode)
├── SO_TAY_KTV.xlsx      # Cơ sở dữ liệu danh mục tra cứu chính
└── requirements.txt     # Các thư viện phụ thuộc
