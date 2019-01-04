---
title: Bitcoin Blockchain
date: 2019-01-04 06:19:00 Z
permalink: "/bitcoin/blockchain"
layout: post
---

# Blockchain

Một file dữ liệu chia sẻ ( dùng chung ) chứa các giao dịch Bitcoin

**Bitcoin Blockchain là gì?**

Blockchain ( ở đây chỉ đề cập đến định nghĩa hẹn blockchain cho bitcoin nói riêng ) là một file chứa danh sách tất cả các transaction về bitcoin đã được tạo ra.

![01-blockchain_file.png](/uploads/01-blockchain_file.png) 

Mọi người trên Bitcoin Network đều sở hữu một bản sao ( a copy ) của file này và thường xuyên cập nhật các transaction mới nhất vào file mà mình đang nắm giữ.

![02-bitcoin_network.png](/uploads/02-bitcoin_network.png)

**Tại sao blockchain lại quan trọng?**

> Blockchain nói cho bạn biết có bao nhiêu bitcoin mà một người sở hữu

Vì blockchain là file chứa danh sách đầy đủ các giao dịch bitcoin nên nó cho phép bạn tìm ra được tại địa chỉ nào có bao nhiêu bitcoin, theo đó bạn sẽ biết được có bao nhiêu bitcoin mà một người sở hữu. Với đặc điểm này blockchain được nhìn nhận giống như một cuốn sổ nhật ký, một cuốn sổ cái (ledger ).

> Ledger ( sổ cái ) là là một thuật ngữ quen thuộc trong chuyên ngành tài chính , kế  toán để chỉ một cuốn sổ ( book ) lưu trữ tất cả các giao dịch tiền bạc ( monetary transaction ) của doanh nghiệp được ghi dưới dạng cột ghi nợ ( debits ) và tín dụng ( credits )

**Tại sao nó được gọi là blockchain?**

Bởi vì các transaction không được thêm vào file một cách riêng lẻ rời rạc mà chúng được bó lại với nhau và thêm vào block. Hơn nữa các block này lại được nối với nhau ( linked ) . Bất cứ thay đổi nào ở các block phía trước ( được tạo ra trước ) sẽ gây ra thay đổi ở các block phía sau nó. Trong hình ảnh dưới đây các block tạo ra trước sẽ nằm ở phía dưới, các block tạo ra sau nằm ở trên.

![03-blocks_chains.png](/uploads/03-blocks_chains.png)

Việc block-ing ( tổ chức các lữu trữ giao dịch theo cấu trúc từng block một ) giúp cho việc chia sẻ bản sao của file blockchain trở nên dễ dàng hơn. Với tốc độ Internet hiện có thì chia sẻ ( dùng chung ) một file với tần suất cập nhật khoảng 10 phút một lần sẽ dễ dàng hơn nhiều so với một file có tần suất cập nhật nhiều lần trong một giây. Con số 10 phút sẽ được giải thích tiếp ở bài sau.

Việc xâu chuối các khối ( block ) lại với nhau là một tính năng bảo mật để chống lại việc làm giả mạo blockchain. Vì thế blockchain hay được dịch ra tiếng Việt là chuỗi khối.

**Blockchain được chia sẻ như thế nào**

File blockchain được chia sẻ bởi các node trên Bitcoin Network giống như các video không có bản quyền được chia sẻ qua mạng ngang hàng ( Peer to Peer-P2P) BitTorrent.

![04-blocks_sharing.png](/uploads/04-blocks_sharing.png)

Các bạn có thể đọc thêm các tài liệu về việc chia sẻ file ngang hàng P2P để hiểu thêm về cơ chế blockchain chia sẻ file ngang hàng trên Bitcoin network.

**Bạn có thể kiếm được một file blockchain ở đâu?**

Bạn có thể được một phiên bản blockchain cho riêng mình bằng cách down load [Bitcoin Client ](https://bitcoin.org/en/download)

Sau khi cài đặt và chạy ứng dụng này thì Client sẽ giúp bạn kết nối với với Bitcoin Network và nó sẽ download blockchain từ trên đó về. Dung lượng của blockchain bitcoin hiện tại là trên 180GB nên bạn sẽ phải tốn thời gian một chút để download hết nó về.\
