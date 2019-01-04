---
title: Nodes
date: 2019-01-04 03:48:00 Z
permalink: bitcoin/nodes
layout: post
---

# Nodes

# `Những máy tính chạy chương trình bitcoin`

![05-nodes_network.png](/uploads/05-nodes_network.png)

Một Node đơn giản chỉ là \*\*một máy tính chạy chương trình Bitcoin\*\*. Nhưng nó không chạy đơn lẻ một mình mà được kết nối với các máy tính khác ( cũng là nodes ) để tạo thành một mạng blockchain ( Network ).

**Một Node sẽ thực hiện chức năng gì ?**

Một node sẽ có 3 công việc

1\. Làm theo các rule ( mệnh lệnh đã được lập trình )

2\. Chia sẻ thông tin

3\. Lưu giữ một bản copy của các giao dịch đã được xác nhận ( confirmed transactions).

**1.  Làm theo các rule**

Mỗi node ( bitcoin client ) được lập trình để tuân theo một loạt các luật ( rule ).  Bằng cách tuân thủ các luật này thì một node có thể kiểm tra được các giao dịch và chỉ chuyển tiếp ( relay ) nếu mọi thứ ok. Còn nếu gặp bất cứ vấn đề gì thì giao dịch sẽ bị bỏ qua

![01-node_rules.png](/uploads/01-node_rules.png)

Ví dụ có 1 rule là một người phải sở hữu một lượng bitcoin bằng hoặc lớn hơn số lượng bitcoin mà họ muốn chuyển đi cho người khác. Nếu như node của bạn nhận được một transaction mà ai đó cố gắng chuyển đi số lượng bitcoin lớn hơn số mà họ có thì transcation này tính là không hợp lệ và không được chuyển đi cho các node khác xử lý tiếp.

**2. Chia sẻ thông tin**

Công việc chính của một node là chia sẻ thông tin với những node khác và thông tin  tinh túy quan trọng nhất mà các node chia sẻ với nhau đó chính là các giao dịch.

Có 2 loại giao dịch mà các node chia sẻ

1\. Các giao dịch mới ( fresh transaction ): là các giao dịch mới được thêm vào mạng lưới ( network )

2\. Các giao dịch đã được xác nhận ( confirmed transaction ): là các giao dịch vừa mới được xác nhận và viết vào file. Các giao dịch này sẽ được chia sẻ trong các *blocks*  ( chứa một tập các transaction ) một cách công khai.

![01-node_transaction_type_sharing.png](/uploads/01-node_transaction_type_sharing.png)

Hiện thời các bạn không cần quan tâm đến sự khác nhau giữa 2 loại nodes này, chúng sẽ được làm rõ trong các bài viết về Mining và  Blocks sau.

**3. Giữ bản copy của các transaction đã được xác nhận**

Như đã đề cập ở trên mỗi Node sẽ giữ một chuỗi các blocks ghi các transaction. Chúng sẽ được tổ chức trong cùng 1 file gọi là blockchain.

![02-node_blockchain.png](/uploads/02-node_blockchain.png)