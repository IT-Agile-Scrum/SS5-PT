# Bài tập phân tích: Ưu tiên hóa Product Backlog bằng MoSCoW

## Bối cảnh

Ứng dụng đặt xe RikkeiGo chuẩn bị phát hành phiên bản cho chương trình “Tháng khuyến mãi”. Đội phát triển có thể làm tối đa **10 điểm** trong Sprint.

## Phần 1 – Hai cách gán nhãn

### Cách 1: Gán nhãn theo mức độ bắt buộc của bản phát hành

- **Must:** Không có hạng mục này thì bản phát hành không thể chạy đúng hoặc gây rủi ro nghiêm trọng cho khách hàng.
- **Should:** Rất có giá trị nhưng vẫn có thể phát hành nếu có giải pháp tạm thời.
- **Could:** Có ích nhưng có thể để sang lần phát hành sau.
- **Won’t:** Chưa làm trong lần phát hành này; phải thông báo rõ cho các bên liên quan.

Cách này tập trung vào tác động thực tế đối với việc phát hành, nên ít bị ảnh hưởng bởi ý kiến của người nói to hơn.

### Cách 2: Gán nhãn theo ý kiến của bộ phận đề xuất

Mỗi bộ phận tự đánh dấu yêu cầu của mình là Must, Should hoặc Could. Sau đó Product Owner chọn theo nhu cầu kinh doanh và thời điểm chương trình.

Cách này nhanh và tận dụng được hiểu biết của từng bộ phận, nhưng dễ xảy ra tình trạng bộ phận nào cũng gọi yêu cầu của mình là Must.

## Phần 2 – So sánh

| Tiêu chí | Cách 1: Theo mức độ bắt buộc | Cách 2: Theo ý kiến bộ phận |
|---|---|---|
| Khách quan khi nhiều bộ phận cùng đề xuất | **(+)** Mọi yêu cầu đều được xét theo cùng câu hỏi: thiếu nó thì bản phát hành có còn chạy đúng không? | **(–)** Nhiều bộ phận có thể cùng tự gắn Must cho yêu cầu của mình. |
| Bảo vệ hạng mục bắt buộc như #1 | **(+)** Lỗi đang thu sai tiền khách được ưu tiên vì có rủi ro trực tiếp và nghiêm trọng. | **(–)** Hạng mục quan trọng có thể bị xếp ngang với yêu cầu “đúng dịp” hoặc yêu cầu được nhiều người ủng hộ. |

## Phần 3 – Áp dụng

Tôi chọn **Cách 1** vì phù hợp hơn với việc chốt phạm vi phát hành và giúp Scrum Master giải quyết bất đồng giữa các bộ phận.

| # | Hạng mục | Nhãn | Điểm | Lý do |
|---:|---|---|---:|---|
| 1 | Sửa lỗi hiển thị sai cước sau khuyến mãi, đang thu sai tiền khách | **Must** | 2 | Nếu không sửa, khách bị tính sai tiền và bản phát hành có rủi ro lớn về tin cậy. |
| 2 | Áp mã khuyến mãi khi đặt xe | **Must** | 2 | Đây là chức năng chính của chương trình “Tháng khuyến mãi”; thiếu nó thì khách không dùng được ưu đãi. |
| 3 | Thanh toán bằng ví RikkeiPay | **Must** | 3 | Ví điện tử giúp hoàn thành luồng thanh toán mới. Việc khách vẫn có thể trả tiền mặt chỉ là giải pháp tạm thời. |
| 4 | Hẹn giờ đặt xe trước | **Should** | 3 | Có giá trị cho khách hàng nhưng bản phát hành vẫn hoạt động nếu tạm thời chưa có tính năng này. |
| 5 | Chat với tài xế | **Could** | 3 | Khách vẫn có thể gọi điện, nên có thể để sau để bảo vệ phạm vi chính của Sprint. |
| 6 | Giao diện trang trí cho chương trình khuyến mãi | **Won’t** | 2 | Giao diện đẹp giúp quảng bá, nhưng thiếu nó bản phát hành vẫn chạy được. Có thể dùng giao diện hiện tại và thông báo đây là phần để sau. |

### Danh sách đưa vào Sprint

Để dùng đủ 10 điểm, Sprint nhận các hạng mục **#1, #2, #3 và #4**:

`2 + 2 + 3 + 3 = 10 điểm`

- Must: #1, #2, #3 = **7 điểm**.
- Should: #4 = **3 điểm**.
- Could: #5 = chưa đưa vào Sprint.
- Won’t: #6 = chưa đưa vào lần phát hành này.

Tỷ lệ Must là **7/10 = 70%**. Tỷ lệ này hơi cao hơn mức khoảng 60% vì các hạng mục có kích thước 2 hoặc 3 điểm, không thể chia nhỏ trong bài toán. Đổi lại, các rủi ro bắt buộc của bản phát hành được bảo vệ đầy đủ.

## Kết luận

Phạm vi Sprint là 4 hạng mục #1–#4, tổng 10 điểm. Mỗi nhãn đều có lý do gắn với bản phát hành “Tháng khuyến mãi”, nên quyết định dễ giải thích với Marketing, Chăm sóc khách hàng và Vận hành.
