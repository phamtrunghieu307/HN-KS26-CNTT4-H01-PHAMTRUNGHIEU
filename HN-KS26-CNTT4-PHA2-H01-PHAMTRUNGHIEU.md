# bai_lam_pha2

# BÀI LÀM PHA 2 – HACKATHON 02

- **Mã đề:** 01
- **Họ tên:Phạm Trung Hiếu**
- **Lớp:KS26-CNTT4**
- **Link repository Pha2:**
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):**

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.
> 

## 4.2. Trích xuất tin nhắn đặt tour ra JSON

**KET QUA AI**

```
[
  {
    "ma_tour": "SP2N",
    "ngay_khoi_hanh": "2026-12-20",
    "nguoi_lon": 2,
    "tre_em": 1,
    "loai_phong": "doi",
    "ghi_chu": null
  },
  {
    "ma_tour": "PQ4N",
    "ngay_khoi_hanh": "2027-01-05",
    "nguoi_lon": 3,
    "tre_em": 0,
    "loai_phong": null,
    "ghi_chu": "1 người ăn chay"
  },
  {
    "ma_tour": null,
    "ngay_khoi_hanh": "2026-12-01",
    "nguoi_lon": 4,
    "tre_em": 0,
    "loai_phong": "doi",
    "ghi_chu": "Ông nội đi xe lăn"
  }
]
```

**Link trò chuyện:**[https://chatgpt.com/share/6afd02b5-636c-83ec-a561-22ad809b393f](https://chatgpt.com/share/6afd02b5-636c-83ec-a561-22ad809b393f)

## 4.3. Báo giá bằng Chain-of-Thought

**KET QUA AI**

```
1. Tiền người lớn:

5 × 3.200.000 = 16.000.000 đồng

2. Tiền trẻ em:
- Trẻ 8 tuổi: 3.200.000 × 70% = 2.240.000 đồng.
- Trẻ 10 tuổi: 3.200.000 × 70% = 2.240.000 đồng.
- Trẻ 3 tuổi: Miễn phí = 0 đồng.
Tổng: 2.240.000 + 2.240.000 = 4.480.000 đồng

3. Tiền tour:

16.000.000 + 4.480.000 = 20.480.000 đồng

4. Giảm giá đoàn:

20.480.000 × 5% = 1.024.000 đồng.

5. Phụ thu:

1 × 800.000 = 800.000 đồng

6. Tổng tiền:

20.480.000 - 1.024.000 + 800.000 = 20.256.000 đồng

[RESULT:20256000đồng]
```

**Link trò chuyện:**[https://chatgpt.com/share/6afd0354-03e0-83ec-9b9b-0656e28b0036](https://chatgpt.com/share/6afd0354-03e0-83ec-9b9b-0656e28b0036)

### b) Kiểm tra kết quả AI

kết luận AI đúng

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```
{
  "loai_su_co": "khach_san",
  "so_khach": 2,
  "so_dem_bi_anh_huong": 2,
  "tom_tat": "2 khách bị chuyển sang khách sạn 3 sao thay vì 4 sao trong 2 đêm đầu, phòng ẩm mốc."
}
```

**Link trò chuyện:**[https://chatgpt.com/share/6afd03ac-9528-83ec-a869-5cdba527f3f3](https://chatgpt.com/share/6afd03ac-9528-83ec-a869-5cdba527f3f3)

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```
Tiêu chí	Điểm	Minh chứng	Đề xuất sửa
Đúng thông tin (50%)	0/5	- Câu sai: “Tour Sa Pa 2N1Đ bên em giá 2.200.000đ/người lớn”. Lý do: Giá chuẩn là 2.400.000đ/người lớn. Sửa: “Tour Sa Pa 2N1Đ bên em có giá 2.400.000đ/người lớn”.

- Câu sai: “Anh huỷ trước 3 ngày thì được hoàn tiền đầy đủ nha anh”. Lý do: Huỷ trước 3 ngày chỉ được hoàn 50%, không phải 100%. Sửa: “Nếu anh huỷ trước ngày đi từ 7 ngày trở lên, công ty hoàn 100%; từ 3 đến 6 ngày hoàn 50%; dưới 3 ngày không được hoàn tiền.”	Cung cấp chính xác giá tour và trình bày đầy đủ cả 3 mốc thời gian hoàn tiền.
Đầy đủ (30%)	1,5/3	- Câu: “Anh cần gì cứ nhắn em nhé!” Lý do: Chưa chủ động mời khách cung cấp ngày đi và số lượng khách để đặt tour. Nhân viên đã đề cập giá và chính sách huỷ nhưng chưa hướng dẫn bước tiếp theo.	“Anh vui lòng cho em xin ngày khởi hành dự kiến và số lượng khách để em hỗ trợ đặt tour ạ.”
Giọng điệu (20%)	1/2	- Câu: “đi rất vui luôn ạ” và “nha anh”. Lý do: Cách diễn đạt hơi suồng sã, thiếu tính chuyên nghiệp trong tư vấn dịch vụ.	Thay bằng cách diễn đạt lịch sự: “Tour có lịch trình tham quan hấp dẫn, hy vọng sẽ mang đến cho anh trải nghiệm thú vị ạ.”
Tổng điểm	2,5/10	Bài làm sai cả giá tour và chính sách huỷ, chưa đầy đủ nội dung tư vấn và còn sử dụng cách diễn đạt thiếu chuyên nghiệp.	Cần kiểm tra thông tin chuẩn, trả lời đủ yêu cầu và chủ động hướng dẫn khách đặt tour.
```

**Link trò chuyện:**[https://chatgpt.com/share/6afd0478-6b94-83ec-8491-1724de3f5c06](https://chatgpt.com/share/6afd0478-6b94-83ec-8491-1724de3f5c06)