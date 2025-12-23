# Introduction
- Giới thiệu ngắn về tính năng, mục tiêu chính, phiên bản và ngày lập kế hoạch.
- <i>Ví dụ</i>:
    - Feature name: Feedback
    - Feature target: Cho phép người dùng gửi ticket báo lỗi hoặc đề xuất cải tiến để admin dễ dàng nhận và xử lý.
    - Version: 2.0
    - Test Plan Version: 1.0
    - Date: 23/12/2025

# Objectives
- Nêu ngắn gọn mục tiêu kiểm thử (chức năng, usability, reliability, error handling…).
- <i>Ví dụ:
Xác minh tính năng Feedback hoạt động đúng, dễ sử dụng, xử lý lỗi tốt và admin có thể quản lý ticket hiệu quả.</i>

# Scope
### In-Scope
- Liệt kê rõ những gì sẽ kiểm thử.
- <i>Ví dụ: </i>
    - Kiểm thử các chức năng chính của tính năng, bao gồm:
    - Luồng người dùng cuối (user portal): gửi ticket, đóng/mở lại ticket, tìm kiếm/lọc ticket, trả lời ticket.

### Out-of-Scope

- Các chức năng, luồng không cần kiểm thử
- <i>Ví dụ</i>:
    - Kiểm thử hiệu năng (performance/load testing).
    - Kiểm thử tương thích thiết bị/di động chi tiết.
# Test Approach
- Nêu phương pháp kiểm thử chính và cách thực hiện (manual hay automation).
- <i>Ví dụ</i>:
    - Phương pháp chính: Equivalence partitioning, Boundary value analysis, State transition testing.
    - Chủ yếu manual execution

# Test Criteria
- Điều kiện bắt đầu và kết thúc kiểm thử.
- <i>Ví dụ</i>:
    - Entry: Môi trường test ổn định, test cases được duyệt.
    - Exit: Đạt 100% coverage các mục in-scope, không còn defect critical/severe.

# Resource

- Danh sách thành viên và phân công trách nhiệm.
- <i>Ví dụ</i>:
    - Team: Duc, Hieu, Anh, Thuy
    - Roles:
        - Build plan & design: Duc
        - Write test cases: Hieu
        - Execute test: Anh, Thuy
        - Report: Duc


# Schedule
- Ước lượng thời gian theo story points hoặc ngày cho từng giai đoạn
- <i>Ví dụ</i>:
    - Build Test Plan: 2 points
    - Build Test Design: 2 points
    - Write Test Cases: 2 points
    - Execute Staging: 3 points
    - Execute Prod: 2 points

# Risks
- Liệt kê ngắn các rủi ro có thể xảy ra.
- <i>Ví dụ</i>:
    - Thay đổi yêu cầu trong sprint.
    - Môi trường test không ổn định.
# Approval
- Người lập kế hoạch và người duyệt.
- <i>Ví dụ</i>:
    - Prepared by: Ducbt
    - Approved by:
    - Date:

# Test Context
- Link gán test context, test design