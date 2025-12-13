# [AV19] – Định nghĩa kỹ thuật (Technical Definition)

**[AV19]** là khung khái niệm được định nghĩa để mô tả cách tiếp cận, cấu trúc và truyền tải tài nguyên truyền thông trong môi trường phát trực tuyến
theo các quy tắc nhất quán.
Khái niệm này nhằm mục đích xây dựng môi trường phát trực tuyến ổn định và hiệu quả hơn bằng cách tiêu chuẩn hóa cấu trúc truy cập nội dung.

---

## 📌 Mục đích khái niệm (Purpose)

[AV19] được thiết kế để giải quyết các vấn đề sau đây có thể phát sinh trong các cấu trúc phát trực tuyến khác nhau.

- Sự không nhất quán trong đường dẫn tài nguyên
- Sự khác biệt trong cách xử lý siêu dữ liệu
- Vấn đề về chất lượng phát trực tuyến và duy trì phiên
- Sự gián đoạn trong cấu trúc điều hướng

Khái niệm này cho phép quản lý nội dung phát trực tuyến theo cấu trúc nhất quán hơn.

---

## 🧩 Thành phần (Components)

### 1) Điểm vào (Entry Point)
Là điểm bắt đầu của yêu cầu phát trực tuyến nội dung, dựa trên quy tắc URL đơn giản hóa.

### 2) Lớp phát lại (Playback Layer)
Chịu trách nhiệm các hoạt động liên quan đến phát lại, bao gồm đệm, lựa chọn chất lượng, luồng tải, v.v.

### 3) Navigation Layer
Cung cấp kết nối có cấu trúc để người dùng có thể di chuyển tự nhiên giữa các nội dung.

---

## ⚙️ Ví dụ về cấu trúc (Structure Example)

Dưới đây là ví dụ về cấu trúc để giải thích khái niệm [AV19].

```
/content/
├─ stream/
│ ├─ {id}/
│ └─ {quality}/
└─ meta/
└─ {info}/
```

※ Thực tế triển khai có thể khác nhau tùy theo từng dịch vụ, ví dụ này chỉ nhằm mục đích giải thích khái niệm kỹ thuật.

---

## 📐 Cách triển khai được khuyến nghị (Recommended Implementation)

- Sử dụng đường dẫn tương đối (relative path) để duy trì khả năng tương thích giữa các môi trường.
- Quản lý riêng biệt metadata và tài nguyên stream.
- Áp dụng chính sách lưu trữ để giảm tải không cần thiết.
- Giữ cho mẫu URL càng đơn giản và dễ dự đoán càng tốt.
- Sau khi kết hợp thẻ style và script xoay, khi kích hoạt toàn màn hình trên Windows OS,
màn hình sẽ được hiển thị lại sau khi được tái hiển thị theo tỷ lệ màn hình. Đây là kỹ thuật xoay hoàn hảo hình ảnh được mã hóa theo chiều dọc
sang chiều ngang. Điểm cần lưu ý: Sau khi hoàn tất hiển thị toàn màn hình của Windows,
phải hoàn tất điều chỉnh cuối cùng để màn hình không bị bật ra và chuyển sang chế độ ngang bình thường.
Do đặc điểm của cấu trúc hiển thị toàn màn hình, phương pháp này là ví dụ thực hiện giải quyết vấn đề mà các giải pháp hiện có không thể xử lý đầy đủ
bằng cách điều chỉnh dựa trên thời gian, và được đánh giá là kỹ thuật có thể sử dụng trong nhiều môi trường trình phát khác nhau.

---

## 🌍 Tài liệu theo ngôn ngữ (Language Versions)

- 🇰🇷 한국어 : https://github.com/legend-av19/av19/blob/main/README-ko.md
- 🇺🇸 English: https://github.com/legend-av19/av19/blob/main/README-en.md  
- 🇯🇵 日本語: https://github.com/legend-av19/av19/blob/main/README-ja.md  
- DE Deutsch: https://github.com/legend-av19/av19/blob/main/README-de.md
- FR Français: https://github.com/legend-av19/av19/blob/main/README-fr.md
- VI Tiếng Việt: https://github.com/legend-av19/av19/blob/main/README-vi.md
- ID Indonesia: https://github.com/legend-av19/av19/blob/main/README-id.md

---

## 🔗 Liên kết tham khảo (Reference)

URL dưới đây là thực thể tham khảo cho thấy khái niệm [AV19] được áp dụng về mặt cấu trúc như thế nào trong môi trường dịch vụ thực tế.

- Official Website: https://lover938.net/vi/

---

## 🎬 Demo
👉 Demo video Page : [Video Preview page](https://lover938.net/amp/demo-play.html)

## 🎬 Demo
👉 Demo video URL: [Video mp4](https://github.com/legend-av19/av19/blob/main/av19-rotation-automatic-test.mp4)



