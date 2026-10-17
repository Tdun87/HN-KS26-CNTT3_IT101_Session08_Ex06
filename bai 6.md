
# Bài 6: Sự cố tài liệu dự án trên GitHub

## 1. Phân tích lỗi của Nam và ưu điểm của Markdown
- **Sai lầm về định dạng (Rich Text):** File Word (`.docx`) là định dạng nhị phân, GitHub không hỗ trợ render trực tiếp trên trình duyệt web cho nhóm xem.
- **Lỗi xung đột (Git Diff & Conflict):** Hệ thống Git không thể so sánh từng dòng (line-by-line) đối với file nhị phân của Word. Chỉ cần một thay đổi nhỏ, Git sẽ báo xung đột toàn bộ tệp khi gộp code.
- **Ưu thế của Markdown:** Là văn bản thô (Plain Text) cực nhẹ, không sợ hỏng tệp do lỗi truyền tải dữ liệu, đồng thời hỗ trợ theo dõi lịch sử thay đổi (Git Diff) hoàn hảo để làm việc nhóm.

## 2. Nội dung chuyển đổi sang `README.md`
# 🌿 Dự án GreenTech: Hệ thống Giám sát Nông nghiệp
> Tự động hóa chăm sóc trang trại Lan ứng dụng IoT.

## Tổng quan hệ thống
- **Mục tiêu:** Giám sát độ ẩm, nhiệt độ và điều khiển máy bơm thời gian thực.
- **Thành phần chính:** Cảm biến điện dung, vi điều khiển ESP32 NodeMCU, hệ thống AI Assistant.

## Hướng dẫn cài đặt nhanh
```python
# Cấu hình ngưỡng vận hành mẫu
TEMP_THRESHOLD = 32.5

def run_system(temp):
    if temp > TEMP_THRESHOLD:
        print("[INFO] Kích hoạt hệ thống phun sương tự động.")
 ```
