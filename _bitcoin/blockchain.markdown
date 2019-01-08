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

Sau khi cài đặt và chạy ứng dụng này thì Client sẽ giúp bạn kết nối với với Bitcoin Network và nó sẽ download blockchain từ trên đó về. Dung lượng của blockchain bitcoin hiện tại là trên 180GB nên bạn sẽ phải tốn thời gian một chút để download hết nó về.

> Trên 180GB này là toàn bộ blockchain chưa tất cả các giao dịch bitcoin từ trước đến giờ ( giao dịch đầu tiên bắt đầu từ ngày 3/1/2019 ).  Việc download toàn bộ blockchain được thực hiện một lần duy nhất, tuy nhiên thì các block mới sẽ thường xuyên được cập nhật, kích thước mỗi block là khoảng 1MB.

Download xong là bạn đã có trong tay một bản sao blockchain hoàn chỉnh. Mỗi lần bạn chạy bitcoin client tức là bạn đã giúp cho việc chia sẻ file blockchain tới mọi người join vào network giúp cho bitcoin trở nên mạnh hơn. 

> Những người khác join vào mạng sẽ download dữ liệu từ các file blockchain lưu trên các node ) giống như mạng torrent người dùng down dữ liệu file video từ các peer khác . Nếu bạn là fan của Torrent, bạn hãy nghĩ bạn bạn là một seeder đang seeding blockchain. 

**File blockchain lưu trữ ở đâu trên máy tính của bạn?**

Blockchain sẽ được lưu trữ trong những files có tên là blk00000.dat,  blk00001.dat, blk00002.dat, v.v. ( Khi kích thước blockchain quá lớn nó sẽ được chia thành nhiều file vật lý, việc chia thành các file chỉ có ý nghĩa lưu trữ về mặt vật lý chứ việc phân chia thành các file không tương ứng với việc phân chia các block, một file không tương ứng với 1 block.

Nơi lưu trữ thì tùy thuộc vào hệ điều hành khác nhau mà bạn đang sử dụng cho máy tính dùng làm node của mình

Linux
\
       /home/\[username\]/.bitcoin/blocks/
\
Windows
\
       C:\\Users\\\[username\]\\AppData\\Roaming\\Bitcoin\\
\
Mac
\
       \~/Library/Application Support/Bitcoin/

Các file .dat này được thiết kế để máy tính có thể đọc hiểu, tuy nhiên khi bạn mở nó ra thì sẽ chỉ thấy dữ liệu toán loạn hầm bà lằng mà thôi nhưng cứ yên tâm đi, đó là dữ liệu về các giao dịch bitcoin 100% đấy.

Nếu bạn muốn có một phiên bản dữ liệu mà con người đọc hiểu được thì hãy có thể sử dụng blockchain browser trên trang này. Chỉ cần post file blk\*.dat lên nó sẽ parse dữ liệu và hiển thị dữ liệu đọc được lên web.