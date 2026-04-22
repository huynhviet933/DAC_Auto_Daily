====================================================================
          HƯỚNG DẪN SỬ DỤNG TOOL DACHAIN INCEPTION
====================================================================

1. YÊU CẦU HỆ THỐNG
--------------------------------------------------------------------
- Cài đặt Node.js phiên bản 18 trở lên.
- Tải toàn bộ source code tool về thư mục.

2. CÀI ĐẶT MÔI TRƯỜNG (CHẠY LỆNH NÀY TRƯỚC)
--------------------------------------------------------------------
Mở Terminal/CMD tại thư mục tool và copy-paste lệnh sau:

npm install axios fs-extra https-proxy-agent chalk@4.1.2 uuid moment-timezone node-machine-id

3. CHUẨN BỊ FILE DỮ LIỆU (TẠO TRONG THƯ MỤC TOOL)
--------------------------------------------------------------------
- wallet.txt      : Mỗi dòng chứa 1 địa chỉ ví (Address).
- proxy.txt       : Mỗi dòng chứa 1 Proxy (http://user:pass@ip:port).
- user_agents.txt : Mỗi dòng chứa 1 User Agent trình duyệt.
- license.txt     : Lưu key bản quyền (Nếu chưa có, tool sẽ hỏi khi chạy).

4. CẤU HÌNH CONFIG.JSON (TỰ SINH KHI CHẠY LẦN ĐẦU)
--------------------------------------------------------------------
{
  "threads_count": 5,           // Số luồng chạy song song
  "stagger_delay_ms": 10000,    // Delay mở luồng mới (10 giây)
  "action_delay_min_ms": 3000,  // Delay nhỏ nhất giữa các bước
  "action_delay_max_ms": 7000,  // Delay lớn nhất giữa các bước
  "account_delay_min_ms": 30000,// Nghỉ tối thiểu khi xong 1 ví
  "account_delay_max_ms": 60000,// Nghỉ tối đa khi xong 1 ví
  "auto_restart_hour_vn": 7     // Tự động chạy lại lúc 7h sáng VN
}

5. CÁCH CHẠY TOOL
--------------------------------------------------------------------
Sử dụng lệnh: 

node p2.js

6. TÍNH NĂNG CHÍNH
--------------------------------------------------------------------
✅ Auto Login & Check-in hàng ngày.
✅ Auto Claim "Early Standard Badge" nhận ngay 250 QE.
✅ Auto Open Crate (Mở hòm) liên tục cho đến khi hết lượt ngày.
✅ Smart Retry: Tự động đổi Proxy & Thử lại khi gặp lỗi kết nối.
✅ Clean Log: Ẩn hoàn toàn các lỗi Proxy, chỉ hiện kết quả thành công.
✅ Resume: Tự động chạy tiếp từ ví bị dừng trước đó (last_index.txt).
✅ License: Tích hợp hệ thống bản quyền xác thực HWID thiết bị.

LƯU Ý: Nếu muốn chạy lại từ ví đầu tiên, hãy xóa file last_index.txt.
====================================================================
Tham Gia NHóm tele : https://t.me/HVchannelss

Tham Gia Discor ( Vip ) : https://discord.gg/gKxvTNu5

Tham gia NHóm VIp Với Chi Phí 1 Tháng 4u - 15u 6thang Lợi ích tham gia nhóm ViP Sẽ được cấp keey sử dụng các tool vip trong discor hỗ trợ Và tham khao Code các tool dự án mà các bạn đề xuất

Gửi Phí tháng vào đây và chụp hình gửi trực tiếp cho tôi tại discor để xác nhận Role VIp ☕ https://huynhviet933.github.io/donate_viet_mmo/ Có thể tặng tôi ít cafe tại đây

Donenat : https://huynhviet933.github.io/donate_viet_mmo/

