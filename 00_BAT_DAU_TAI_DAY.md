# BẮT ĐẦU TẠI ĐÂY — Bài thực hành dữ liệu đặt phòng khách sạn

> Đọc trong 3 phút. Tài liệu đầy đủ và **chính thức** là `De_bai_Khach_san.docx`.

## Bạn sẽ làm gì?

Nhận một tệp dữ liệu đặt phòng của hai khách sạn **có lỗi cài sẵn** (10.325 dòng × 24 cột) và biến nó thành:

| Sản phẩm | Số lượng |
|---|---|
| Bảng dữ liệu sạch có truy vết (gồm bảng đặt phòng và bảng tổng hợp theo tháng) | 5 tệp CSV |
| Câu hỏi phân tích (hủy phòng, mùa vụ, lead time, giá phòng, lưu trú…) | 10 câu |
| Biểu đồ đạt chuẩn | 8 hình |
| Insight có bằng chứng | 6 insight |
| Báo cáo | 8–12 trang |

Không cần học máy. Không cần tài khoản Kaggle. Chỉ cần Python, pandas, matplotlib.

## 5 bước khởi động (15 phút)

1. **Đọc trang 2 của đề** (“Bài tập trong một trang”) và **Mục 3** (sơ đồ quy trình).
2. **Mở notebook** `hotel_student_starter.ipynb`
   - *Colab:* File → Upload notebook; bảng 📁 Files → tải `data/hotel_bookings_dirty.csv` lên.
   - *Máy cá nhân:* giữ nguyên cấu trúc thư mục này, mở notebook tại đây.
3. **Chạy ô 0.1 và 0.2.** Phải thấy: `✅ Đầu vào đúng 10.325 dòng × 24 cột`.
4. **Phân công** theo Mục 14 của đề; đặt lịch 5 buổi.
5. **Bắt đầu Giai đoạn A** — khảo sát, *chưa sửa gì*.

## Quy trình 5 giai đoạn

```
A Khảo sát  →  B Làm sạch (B1–B8)  →  C Bảng sạch & kiểm tra  →  D 10 câu hỏi  →  E Insight & nộp
  ≈ 2 giờ          ≈ 3,5 giờ                ≈ 2 giờ                  ≈ 3 giờ          2–5 giờ
```

Mỗi giai đoạn trong notebook có **thẻ nhiệm vụ** (mục tiêu, các bước, bẫy thường gặp) và **ô tự kiểm tra** in ✅ / ❌.

## Ba nguyên tắc không được vi phạm

- ❌ **Không sửa tay** tệp CSV, không thay bằng bộ dữ liệu gốc sạch.
- ❌ **Không đoán dữ liệu** — không sửa được bằng bằng chứng thì để thiếu và ghi lý do; không điền trung bình.
- ❌ **Không kết luận vượt dữ liệu** — chỉ có 2 khách sạn ở Bồ Đào Nha, 2015–2017; không suy ra nguyên nhân hủy phòng; `adr` không phải doanh thu.

## Trước khi nộp

```bash
python tools/kiem_tra_nop_bai.py NhomXX_KhachSan
```

Nộp `NhomXX_KhachSan.zip` khi công cụ **không còn ❌**. Cấu trúc thư mục bài nộp: Mục 12 của đề.
