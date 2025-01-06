Giới thiệu

Đây là một dự án máy học giúp phân loại tin nhắn SMS thành hai loại: spam (tin nhắn rác) và ham (tin nhắn bình thường). Ta sử dụng thư viện TensorFlow để xây dựng mô hình, với quy trình xử lý dữ liệu văn bản từ bước tiền xử lý đến huấn luyện và đánh giá kết quả.

Dự án có gì hay?

  Phân loại tin nhắn tự động: Giúp bạn nhanh chóng nhận biết tin nhắn nào là rác.
  Xử lý văn bản chuẩn chỉnh:
  
      Chuyển đổi từ thành số (tokenization) và làm đều độ dài tin nhắn (padding).
      Gắn nhãn ham là 0, spam là 1.
      
  Mô hình học sâu:
  
      Dùng lớp nhúng (embedding) để hiểu ý nghĩa từ.
      Lớp dense giúp dự đoán chính xác.
      
  Dễ dùng: Chỉ cần gọi hàm là có thể kiểm tra tin nhắn.

### Ví dụ kết quả

Dưới đây là một số tin nhắn và dự đoán từ mô hình:

| Tin nhắn                                                                                     | Dự đoán    |
|---------------------------------------------------------------------------------------------|------------|
| urgent! call 09066350750 from your landline...                                               | spam       |
| message important information for o2 user...                                                | spam       |
| i dont want to go. can we try it a different day?                                            | ham        |
| our new mobile video service is live...                                                     | spam       |
| shit that is really shocking and scary, cant imagine for a second...                        | ham        |
| i'll bring it tomorrow. don't forget the milk.                                              | ham        |
| Congratulations! You have won a $1000 cash prize. Call now to claim.                        | spam       |

