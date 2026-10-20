# Bắt đầu với A1 Marketing Orchestrator

Đây là bộ Skill MVP cho A1 gồm hướng dẫn điều phối, bộ quy tắc, mẫu đầu ra, tóm tắt baseline 2026–2027 và Workbench có sáu nút thao tác.

## Dùng Workbench

1. Mở `assets/A1-Workbench.html` bằng trình duyệt.
2. Chọn một trong sáu thao tác: Kế hoạch tháng, Tạo Campaign/Batch, Giao việc, Kiểm tra ngân sách, Rà Gate/ngoại lệ, Báo cáo kết quả.
3. Điền thông tin đầu vào và trạng thái phê duyệt của mục tiêu/ngân sách; để trống trường chưa biết.
4. Chọn **Tạo yêu cầu cho Skill A1**, sau đó **Sao chép yêu cầu**.
5. Dán yêu cầu vào cuộc trò chuyện đang có hướng dẫn A1 này (hoặc môi trường Skill đã nạp `SKILL.md` và thư mục `references/`). AI sẽ tạo output theo mẫu phù hợp.

Workbench chạy cục bộ trong trình duyệt. Sáu nút tạo prompt và gói JSON; chúng không tự gọi mô hình AI, lưu dữ liệu lên máy chủ, ghi Airtable/Drive/CRM, đăng bài hay chạy quảng cáo.

## Điều kiện trước khi coi là tự động hóa vận hành

- Xác nhận người có quyền duyệt và bảng phân công theo Campaign/Batch có ngày hiệu lực.
- Technical Owner chốt model/tenant/cost cap, quyền đọc/ghi và nơi lưu hồ sơ.
- Business Owner/Technical Owner thống nhất cách ánh xạ bốn bước kiểm soát trong A1 với hai Approval Event của manifest Airtable PREPARE.
- Gắn nguồn hiện hành và bằng chứng duyệt cho mục tiêu tháng, ngân sách, KPI, kênh và đầu ra.
- Chạy UAT các tình huống trong sheet A1 trước khi kết nối hệ thống thật.

## Lưu ý về baseline

Các lịch và số ngân sách trong `references/planning-baseline.md` là đề xuất của deck 2026–2027. Chỉ thay nhãn thành **ĐÃ XÁC NHẬN** khi có hồ sơ phê duyệt đúng phạm vi và thời hạn.
