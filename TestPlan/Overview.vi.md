# Tổng Quan Về Test Strategy, Test Plan, Test Design
Trong kiểm thử phần mềm (software testing), ba khái niệm này là nền tảng để lập kế hoạch và thực hiện kiểm thử hiệu quả. Chúng được xây dựng theo thứ tự: Strategy (chiến lược tổng thể) → Plan (kế hoạch chi tiết) → Design (thiết kế cụ thể). Dưới đây là tổng quan ngắn gọn, dễ nhớ.

### Test Strategy và Test Plan
||Test Strategy|Test Plan|
|-|-|-|
|Định nghĩa|Tài liệu cấp cao, mô tả cách tiếp cận tổng thể cho kiểm thử toàn dự án.|Tài liệu chi tiết, mô tả cách thực hiện kiểm thử cụ thể cho một release hoặc giai đoạn.|
|Mục đích|Định hướng tổng quát, quản lý rủi ro, phù hợp mô hình phát triển (Agile/Waterfall).|Lập kế hoạch hoạt động, phân bổ nhiệm vụ, theo dõi tiến độ và chất lượng sản phẩm.|
|Nội dung chính|Mục tiêu, phạm vi, tài nguyên sơ bộ, chiến lược rủi ro.|Giới thiệu, tài nguyên cụ thể, lịch trình, loại kiểm thử, deliverables.|
|Đặc điểm|Cấp cao, ít thay đổi, hướng dẫn tổng quát.|Chi tiết, có thể thay đổi theo dự án, thực tế hơn.|
|Ưu/Nhược|Ưu: Linh hoạt; Nhược: Không chi tiết thực thi.|Ưu: Hướng dẫn cụ thể; Nhược: Tốn thời gian cập nhật.|

- **Test Strategy**: Sử dụng ở giai đoạn lập kế hoạch dự án sớm, khi cần khung tổng thể cho toàn bộ quy trình kiểm thử (ví dụ: dự án lớn, đa giai đoạn). Lý tưởng cho việc định hướng dài hạn và quản lý rủi ro cao cấp.
- **Test Plan**: Sử dụng ở giai đoạn planning chi tiết, cho từng sprint/release cụ thể (ví dụ: trong Agile, Sprint Planning). Phù hợp khi cần kế hoạch thực thi ngay lập tức và theo dõi tiến độ.

# Test Strategy (Chiến Lược Kiểm Thử)
- **Định nghĩa**: Tài liệu cấp cao mô tả cách tiếp cận tổng thể cho kiểm thử, dựa trên yêu cầu dự án, rủi ro và mục tiêu kinh doanh. Nó định hướng toàn bộ quy trình kiểm thử mà không đi sâu vào chi tiết.
- **Mục đích**:
    - Xác định phạm vi kiểm thử (scope), loại kiểm thử (manual/automation), công cụ, và tiêu chí thành công/thất bại.
    - Đảm bảo phù hợp với mô hình phát triển (Agile, Waterfall) và quản lý rủi ro.

- **Nội dung chính**:
    - Mục tiêu kiểm thử.
    - Phạm vi (in-scope/out-of-scope).
    - Tài nguyên (nhân sự, công cụ như Selenium, JIRA).
    - Lịch trình sơ bộ và tiêu chí exit/entry.
    - Chiến lược rủi ro (risk-based testing).

- **Đặc điểm**: Cấp cao, ít thay đổi, thường do Test Manager soạn thảo. Ví dụ: "Ưu tiên automation cho regression testing trong Agile".
- **Ưu/Nhược**: Ưu: Hướng dẫn tổng quát; Nhược: Không chi tiết thực thi.
- **Sử dụng**: Giai đoạn lập kế hoạch dự án sớm.

# Test Plan (Kế Hoạch Kiểm Thử)
- **Định nghĩa**: Tài liệu chi tiết dựa trên Test Strategy, mô tả cách thực hiện kiểm thử cụ thể cho một dự án hoặc release.
- **Mục đích**:
    - Lập kế hoạch hoạt động, phân bổ nhiệm vụ, và theo dõi tiến độ để đảm bảo chất lượng sản phẩm.
    - Xác định các rủi ro cụ thể và cách giảm thiểu.

- **Nội dung chính**:
    - Giới thiệu (mục tiêu, phạm vi).
    - Tài nguyên (team, môi trường test).
    - Lịch trình và milestones.
    - Các loại kiểm thử (unit, integration, system, acceptance).
    - Tiêu chí suspension/resumption.
    - Danh sách deliverables (test cases, reports).

- **Đặc điểm**: Chi tiết hơn Strategy, có thể thay đổi theo dự án. Ví dụ: "Test 80% coverage với 500 test cases trong 2 tuần".
- **Ưu/Nhược**: Ưu: Hướng dẫn thực tế; Nhược: Tốn thời gian cập nhật nếu dự án thay đổi.
- **Sử dụng**: Giai đoạn planning chi tiết, thường trong Sprint Planning (Agile).

# Test Design (Thiết Kế Kiểm Thử)
- **Định nghĩa**: Quá trình tạo ra các yếu tố kiểm thử cụ thể từ requirements, bao gồm test scenarios, test cases, và data test.
- **Mục đích**:
    - Đảm bảo kiểm thử bao quát đầy đủ (coverage), phát hiện lỗi sớm.
    - Chuyển yêu cầu thành các bài test thực thi được.

- **Nội dung chính**:
    - Phân tích requirements → Tạo test scenarios (tổng quát).
    - Thiết kế test cases (chi tiết: steps, input, expected output).
    - Sử dụng kỹ thuật: Equivalence Partitioning, Boundary Value Analysis.
    - Test data và môi trường setup.

- **Đặc điểm**: Tập trung vào "làm thế nào" để test, thường automated nếu có thể. Ví dụ: Từ requirement "Đăng nhập", thiết kế 10 test cases cho positive/negative cases.
- **Ưu/Nhược**: Ưu: Tăng hiệu quả phát hiện bug; Nhược: Cần kinh nghiệm để tránh dư thừa.
- **Sử dụng**: Giai đoạn design/test execution, liên kết với Test Plan.