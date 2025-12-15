# Test Plan là gì?
Test Plan (Kế hoạch kiểm thử) là một tài liệu có cấu trúc chi tiết, định nghĩa các mục tiêu, quy trình, chiến lược và nguồn lực cần thiết cho một dự án kiểm thử phần mềm. Test Plan đóng vai trò như một bản thiết kế (blueprint) cho hoạt động kiểm thử phần mềm, đảm bảo phương pháp tiếp cận có hệ thống và tổ chức.

Một Test Plan được xây dựng tốt đảm bảo rằng tất cả các bên liên quan trong quá trình phát triển phần mềm hiểu rõ về mục tiêu kiểm thử, timeline và effort cần thiết. Nó cũng đảm bảo mọi khía cạnh kiểm thử cho từng thành phần được xử lý kỹ lưỡng và thực thi có hệ thống.

# Tại sao Test Plan quan trọng?
### Lợi ích chính của Test Plan:
1. **Ngăn ngừa lỗi sau khi release**: Chi phí để sửa lỗi sau khi release cao hơn rất nhiều so với phát hiện sớm trong quá trình testing
2. **Xác định mục tiêu rõ ràng**: Xác định chính xác những gì cần được kiểm thử và đảm bảo phù hợp với yêu cầu
3. **Đảm bảo coverage toàn diện**: Bao quát cả khía cạnh functional và non-functional để giảm thiểu rủi ro
4. **Tối ưu hóa phân bổ nguồn lực**: Phân công vai trò, công cụ và lịch trình hiệu quả
5. **Cải thiện độ chính xác và hiệu quả**: Chuẩn hóa quy trình và nâng cao khả năng theo dõi lỗi
6. **Giao tiếp trong team hiệu quả hơn**: Rõ ràng ai làm việc gì, cộng tác với nhau như thế nào.
7. **Đảm bảo tuân thủ**: Tuân theo các tiêu chuẩn ngành và yêu cầu quy định

# Các loại Test Plan
1. **Master Test Plan**
- Tài liệu cấp cao định nghĩa phương pháp kiểm thử tổng thể cho toàn bộ dự án. Bao gồm mục tiêu, phạm vi, phương pháp luận, nguồn lực và timeline, đảm bảo tính nhất quán trong tất cả hoạt động kiểm thử.

2. **Specific Test Plan (Phase Test Plan)**
- Tập trung vào các loại kiểm thử riêng lẻ như:
    - **Performance Test Plan**: Chi tiết về load testing, stress testing
    - **Security Test Plan**: Hướng dẫn kiểm tra bảo mật
    - **UAT Test Plan**: Dựa trên yêu cầu người dùng
    - **System Test Plan**: Dựa trên đặc tả kỹ thuật
3. **Level Test Plan**
    - **Unit Test Plan**: Cho kiểm thử đơn vị
    - **Integration Test Plan**: Cho kiểm thử tích hợp
    - **System Test Plan**: Cho kiểm thử hệ thống
    - **Acceptance Test Plan**: Cho kiểm thử chấp nhận

# Các thành phần chính của Test Plan
Một Test Plan hoàn chỉnh cần bao gồm các thành phần sau:

1. **Test Plan Identifier**: Mã định danh duy nhất cho Test Plan

2. **Introduction**: Giới thiệu tổng quan về dự án và mục đích của tài liệu

3. **Test Items**: Danh sách các thành phần, tính năng cần kiểm thử

4. **Features to be Tested**: Chi tiết các tính năng sẽ được kiểm thử

5. **Features Not to be Tested**: Các tính năng không nằm trong phạm vi kiểm thử

6. **Testing Approach/Strategy**: Phương pháp và chiến lược kiểm thử

7. **Pass/Fail Criteria**: Tiêu chí để xác định test case pass hay fail

8. **Suspension and Resumption Criteria**: Điều kiện tạm dừng và tiếp tục kiểm thử

9. **Test Deliverables**: Các sản phẩm bàn giao của quá trình kiểm thử

10. **Testing Tasks**: Các nhiệm vụ kiểm thử cụ thể

11. **Environmental Needs**: Yêu cầu về môi trường kiểm thử

12. **Responsibilities**: Trách nhiệm của từng thành viên

13. **Schedule**Lịch trình kiểm thử chi tiết

14. **Risk and Mitigation**: Rủi ro và biện pháp giảm thiểu

15. **Approvals**: Phê duyệt từ các bên liên quan

# 8 bước viết Test Plan chi tiết
### Bước 1: Phân tích sản phẩm (Product Analysis)
Trước khi bắt đầu testing, cần hiểu sâu về phần mềm, mục đích và chức năng của nó.

**Cách thực hiện:**

- **Thảo luận với stakeholders**: Phỏng vấn khách hàng, developer, designer để thu thập thông tin
- **Xem xét tài liệu**: Nghiên cứu tài liệu dự án, đặc tả kỹ thuật và yêu cầu người dùng
- **Tìm hiểu sản phẩm**: Tự trải nghiệm phần mềm để hiểu các tính năng, luồng người dùng và điểm yếu tiềm ẩn
Câu hỏi cần trả lời:

**Người dùng là ai?**
- Sản phẩm giải quyết vấn đề gì?
- Cách thức hoạt động như thế nào?
- Yêu cầu kỹ thuật và hạ tầng?
### Bước 2: Phát triển chiến lược kiểm thử (Test Strategy Development)
Test Strategy là tài liệu cấp cao xác định phương pháp tiếp cận kiểm thử tổng thể.

**1. Xác định phạm vi (Scope Definition)**
- **In-scope (Trong phạm vi)**:
    - Functional testing cho tất cả module chính
    - API testing cho các endpoint quan trọng
    - UI/UX testing trên các browser phổ biến
    - Security testing cho authentication và authorization
- **Out-of-scope (Ngoài phạm vi)**:
    - Hardware testing
    - Third-party integration ngoài hệ thống
    - Load testing (nếu ngân sách hạn chế)

**2. Lựa chọn loại kiểm thử (Testing Types Selection)**
- **Ưu tiên các loại testing dựa trên:**
    - Tính chất ứng dụng: Web, Mobile, Desktop
    - Yêu cầu nghiệp vụ: Banking cần security cao, E-commerce cần performance tốt
    - Ngân sách và timeline
- **Ma trận ưu tiên Testing Types:**

|Loại Testing|Ưu tiên|Lý do|
|-|-|-|
|Functional|Cao|Core business logic|
|Security|Cao|Dữ liệu nhạy cảm|
|Usability|Trung bình|User experience|
|Performance|Trung bình|Phụ thuộc traffic|
|Compatibility|Thấp|Target audience cụ thể|

**3. Quản lý rủi ro (Risk Management)**
Bảng phân tích rủi ro:
|Rủi ro|Xác suất|Tác động|Giải pháp|
|-|-|-|-|
|Code chậm/ delay|Cao|Cao|Buffer time 20%, daily standup|
|Thiếu test data|Trung bình|Cao|Chuẩn bị data generator tool|
|Môi trường không ổn định|Cao|Trung bình|Backup environment, monitoring|
|Thiếu nhân sự có kĩ năng tốt|Thấp|Cao|Training plan, outsourcing backup|


### Bước 3: Xác định mục tiêu kiểm thử (Test Objectives)
Mục tiêu cần SMART (Specific, Measurable, Achievable, Relevant, Time-bound).

**Ví dụ mục tiêu cụ thể:**

1. **Functional Testing:**
    - Xác minh 100% các yêu cầu về nghiệp vụ được implement chính xác.
    - Kiểm tra tất cả workflow chính hoạt động mượt mà, không bị block
2. **Performance Testing:**
    - Response time < 2 giây cho 95% transactions
    - Hệ thống xử lý được 1000 concurrent users
3. **Security Testing:**
    - Không có vulnerability critical theo OWASP Top 10
    - Compliance với PCI-DSS (cho payment)
4. **Usability Testing:**
    - Task completion rate > 90%
    - User satisfaction score > 4/5
### Bước 4: Định nghĩa tiêu chí kiểm thử (Test Criteria)
- **Entry Criteria (Điều kiện bắt đầu)**
    - Code development hoàn thành cho module cần test
    - Unit test pass rate > 80%
    - Test environment sẵn sàng
    - Test data đã được chuẩn bị
    - Test cases được review và approve
- **Suspension Criteria (Tiêu chí tạm dừng)**
    - Blocker bugs > 5 chưa được fix
    - Critical functionality không hoạt động
    - Test environment down > 4 giờ
    - 40% test cases failed trong smoke test
- **Exit Criteria (Tiêu chí kết thúc)**
    - Định lượng:
        - Test coverage ≥ 95%
        - Pass rate ≥ 90%
        - Không còn bug Critical/Blocker
        - Bug Major ≤ 5 và có workaround
    - Định tính:
        - Các bên liên quan chấp thuận
        - Release notes đã được hoàn thiện
        - Hoàn thành knowledge transfer
### Bước 5: Lập kế hoạch nguồn lực (Resource Planning)
Nguồn lực con người
Công cụ và Infrastructure
### Bước 6: Thiết lập môi trường test (Test Environment Setup)
### Bước 7: Lập lịch trình và ước lượng (Scheduling & Estimation)
### Bước 8: Xác định sản phẩm bàn giao (Test Deliverables)
**Deliverables Timeline**

- **Pre-Testing Phase:**
    - Test Plan Document (Week 1)
    - Test Strategy Document (Week 1)
    - Test Case Specifications (Week 2-3)
    - Test Data Requirements (Week 2)
    - Traceability Matrix template (Week 2)
- **During Testing Phase:**
    - Daily Test Execution Report
    - Weekly Defect Summary
    - Test Execution Logs
    - Updated Traceability Matrix
    - Environment Health Report
- **Post-Testing Phase:**
    - Test Summary Report
    - Defect Analysis Report
    - Test Metrics Dashboard
    - Lessons Learned Document
    - Test Closure Report
    - Sign-off Document

Nguồn: [BetterBytesAcademy-TestPlan](https://academy.betterbytesvn.com/test-plan-la-gi-huong-dan-toan-dien-cach-viet-test-plan-hieu-qua/#test-plan-l%C3%A0-g%C3%AC)