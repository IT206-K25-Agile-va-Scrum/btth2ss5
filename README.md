# BÁO CÁO THỰC HÀNH: PHÂN LOẠI ƯU TIÊN MoSCoW VÀ XÂY DỰNG DEFINITION OF DONE - DỰ ÁN GOMART

> 👤 **Học viên:** Đỗ Hoàng Sơn | **Mã SV:** PTIT-HCM-066
> 🏫 **Môn học:** IT206-K25-Agile-va-Scrum

---

## Nhiệm vụ 1: Lập bảng 4 nhóm MoSCoW cho 12 User Story

Sau khi phân tích cẩn thận 12 hạng mục trong Product Backlog của dự án GoMart cho bản Release 1.0 (quỹ thời gian 2 Sprint, mỗi Sprint 2 tuần với team 5 người), tôi đã phân loại các User Story vào 4 nhóm MoSCoW đảm bảo tính logic và khả thi thực tế.

| Nhóm MoSCoW | Mã User Story | Tên User Story | Lý giải ngắn gọn / Hướng xử lý |
| --- | --- | --- | --- |
| Must have | US-01 | Dang ky / dang nhap bang so dien thoai | Thiếu tính năng này thì hệ thống không biết người dùng là ai để lưu đơn hàng. |
| Must have | US-02 | Chon sieu thi trong ban kinh 3km | Khách hàng bắt buộc phải chọn siêu thi gần nhất để nhân viên đi chợ có điểm xuất phát. |
| Must have | US-04 | Gio hang va dat don di cho | Nghiệp vụ cốt lõi của ứng dụng: gom sản phẩm và gửi yêu cầu đi chợ hộ. |
| Must have | US-05 | Tinh tong tong tien don + phi giao hang tu dong | Bắt buộc phải tính đúng tiền hàng cộng phí ship thì khách mới biết cần thanh toán bao nhiêu. |
| Should have | US-03 | Tim kiem san pham theo ten | Rất hữu ích để tìm nhanh sản phẩm nhưng nếu chưa có thì khách có thể lướt danh mục (dù hơi mất thời gian). |
| Should have | US-06 | Thanh toan bang the ATM noi dia | Quan trọng cho thanh toán điện tử nhưng Release 1.0 đã có tiền mặt, nên xếp vào nhóm nên có. |
| Should have | US-07 | Ap dung ma freeship | Thu hút người dùng nhưng không chặn đứng luồng đặt đơn cơ bản. |
| Should have | US-09 | Danh gia nguoi di cho ho 5 sao | Giúp kiểmm soát chất lượng dịch vụ nhưng làm sau khi luồng đặt đơn đã mượt mà. |
| Could have | US-08 | Chat voi nguoi di cho ho | Tính năng bổ trợ nâng cao trải nghiệm, có thể hoãn lại nếu thiếu thời gian. |
| Could have | US-10 | Chon nguoi di cho ho yeu thich | Tiện ích phụ, chỉ làm khi Sprint còn dư thời gian ở phút chót. |
| Won't have | US-11 | Dat don di cho dinh ky hang tuan | Chưa làm trong Release 1.0 do phức tạp về logic định kỳ và thanh toán tự động. |
| Won't have | US-12 | Mo rong sang dich vu giao thuoc | Nằm ngoài phạm vi bài toán đi chợ thực phẩm tươi sống của bản phát hành đầu tiên. |

## Nhiệm vụ 2: Lý giải các User Story thuộc nhóm Must have

Dưới đây là các câu lý giải cụ thể cho từng User Story nằm trong nhóm Must have. Nếu thiếu bất kỳ hạng mục nào dưới đây, ứng dụng GoMart sẽ không thể vận hành hoặc không thể phát hành ra thị trường:

- US-01 (Đăng ký / đăng nhập bằng số điện thoại): Thiếu tính năng này, hệ thống hoàn toàn mù tịt về danh tính khách hàng, không thể lưu trữ lịch sử đơn hàng cũng như liên lạc khi giao hàng.
- US-02 (Chọn siêu thị trong bán kính 3km): Không thể bỏ qua vì đây là căn cứ xác định nguồn hàng và phân công nhân viên đi chợ tại cơ sở gần nhất.
- US-04 (Giỏ hàng và đặt đơn đi chợ): Đây là huyết mạch của sản phẩm. Không có giỏ hàng và nút đặt đơn thì ứng dụng không có chức năng cốt lõi để kinh doanh.
- US-05 (Tính tổng tiền đơn + phí giao hàng tự động): Thiếu cơ chế tính tiền tự động thì giao dịch tài chính bị tắc nghẽn, khách hàng và hệ thống không thể khớp lệnh thanh toán.

## Nhiệm vụ 3: Liệt kê tập MVP của Release 1.0

Tập sản phẩm khả thi tối thiểu (MVP - Minimum Viable Product) của Release 1.0 chính là toàn bộ nhóm Must have đã xác định ở trên. Tổng cộng gồm đúng 4 User Story: US-01, US-02, US-04 và US-05.

Việc giới hạn đúng 4 hạng mục này giúp team 5 người tập trung toàn lực hoàn thành trong 2 Sprint ngắn ngủi, tránh việc ôm đồm dẫn đến trễ tiến độ.

## Nhiệm vụ 4: Phân tích các User Story nhóm Won't have

Đối với các User Story được xếp vào nhóm Won't have (US-11 và US-12), tôi đã lên kế hoạch rõ ràng về thời điểm đưa vào các bản release tiếp theo cũng như điều kiện để xem xét lại:

| Mã US | Tên User Story | Dự kiến đưa vào Release mấy | Điều kiện để xem xét lại |
| --- | --- | --- | --- |
| US-11 | Dat don di cho dinh ky hang tuan | Release 2.0 | Release 1.0 đã vận hành ổn định, lượng người dùng quay lại (Retention Rate) cao và hệ thống đã tích hợp ví điện tử / cổng thanh toán định kỳ. |
| US-12 | Mo rong sang dich vu giao thuoc | Release 3.0 | Mảng đi chợ thực phẩm tươi sống đã đạt điểm hòa vốn, team mở rộng thêm nhân sự và có sự đồng thuận pháp lý về việc kinh doanh dược phẩm trực tuyến. |

## Nhiệm vụ 5: Xây dựng bảng Definition of Done (DoD) cho Sprint

Dựa trên năng lực thực tế của một Scrum Team gồm 5 thành viên làm việc trong 2 tuần mỗi Sprint, tôi thiết lập bảng Definition of Done (DoD) gồm 5 tiêu chuẩn bắt buộc áp dụng cho mọi User Story trước khi được coi là Hoàn thành (Done):

| STT | Tiêu chuẩn DoD | Mô tả chi tiết kiểm tra | Trách nhiệm |
| --- | --- | --- | --- |
| 1 | Code Review | Toàn bộ mã nguồn của User Story phải được review và approve bởi ít nhất 1 thành viên khác trong team. | Developer |
| 2 | Unit Test Pass | Viết unit test cho các hàm logic chính, độ bao phủ code (Coverage) đạt tối thiểu 70%. | Developer |
| 3 | Functional Testing | Đã kiểm thử chức năng trên môi trường Staging, không còn lỗi nghiêm trọng (Blocker/Critical). | QA / Tester |
| 4 | UI/UX Check | Giao diện hiển thị đúng thiết kế trên cả 2 nền tảng phổ biến (Mobile Web hoặc Responsive App). | Designer / Dev |
| 5 | Product Owner Acceptance | Product Owner trực tiếp nghiệm thu tính năng và xác nhận đạt yêu cầu Acceptance Criteria. | Product Owner |

## Nhiệm vụ 6: Bảng so sánh Acceptance Criteria (AC) và Definition of Done (DoD)

Để phân biệt rạch ròi giữa AC và DoD, tôi đã lập bảng so sánh chi tiết theo 4 tiêu chí cốt lõi, kèm ví dụ cụ thể lấy từ dự án GoMart:

| Tiêu chí so sánh | Acceptance Criteria (AC) | Definition of Done (DoD) |
| --- | --- | --- |
| Phạm vi áp dụng | Áp dụng riêng cho từng User Story cụ thể. | Áp dụng chung cho tất cả mọi User Story trong Sprint. |
| Bản chất | Mô tả chi tiết các điều kiện nghiệp vụ để tính năng đó hoạt động đúng ý muốn. | Mô tả tập hợp các công việc kỹ thuật và chất lượng cần hoàn thành để coi là 'Xong'. |
| Người quyết định | Product Owner phối hợp cùng Business Analyst và Team. | Toàn bộ Scrum Team cùng thống nhất. |
| Ví dụ minh họa GoMart | Khi đơn chưa đủ 150.000đ, hệ thống ẩn nút 'Áp dụng mã freeship'. | Toàn bộ code phải được review bởi ít nhất 1 thành viên khác. |

## Nhiệm vụ 7: Xếp loại các phát biểu

Dưới đây là phần phân loại chính xác cho 4 phát biểu được đề bài đưa ra:

- (1) 'Khi bấm Đặt đơn, hệ thống hiển thị mã đơn hàng trong vòng 3 giây' -> Thuộc nhóm Acceptance Criteria (Đặc tả điều kiện nghiệp vụ riêng của US đặt đơn).
- (2) 'Toàn bộ code phải được review bởi ít nhất 1 thành viên khác' -> Thuộc nhóm Definition of Done (Tiêu chuẩn chất lượng kỹ thuật áp dụng chung).
- (3) 'Độ bao phủ unit test của sprint đạt trên 70%' -> Thuộc nhóm Definition of Done (Tiêu chuẩn kiểm thử chung cho mọi hạng mục).
- (4) 'Khi đơn chưa đủ 150.000đ, hệ thống ẩn nút 'Áp dụng mã freeship'' -> Thuộc nhóm Acceptance Criteria (Điều kiện logic cụ thể của US mã giảm giá).

## Nhiệm vụ 8: Lưu bài nộp

Bài thực hành đã được hoàn thiện đầy đủ các nội dung theo đúng yêu cầu, định dạng tên tệp chuẩn là gomart_moscow_dod.docx và sẵn sàng nộp lên kho lưu trữ GitHub Organization IT206-K25-Agile-va-Scrum.

---

## 📁 Danh sách tệp tin nộp bài trong Repository
- 📝 `btth2.docx`: Báo cáo tài liệu phân tích nghiệp vụ hoàn chỉnh.
