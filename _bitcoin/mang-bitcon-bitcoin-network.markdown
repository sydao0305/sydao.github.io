---
title: Mạng bitcon( Bitcoin Network)
date: 2019-01-08 08:10:00 Z
permalink: "/bitcoin/network"
---

# Bitcoin Network

Một mạng máy tính chạy các chương trình bitcoin

Mạng bitcoin là gì?

Mạng bitcoin được hình thành bởi tất cả những người chạy phần mềm bitcoin ( bitcoin client ).

![01-software_network.png](/uploads/01-software_network.png)

**Mạng bitcoin làm công việc gì?**

![02-software_network_talking.png](/uploads/02-software_network_talking.png)

Mọi người ( bitcoin clients ) nói chuyện với nhau. Nói chuyện với nhau ở đây hàm nghĩa rằng thông tin được truyền từ bitcoin client này sang các client khác trong mạng. Công việc này được hoàn thiện khi client này gửi tới client khác một thông báo ( message ). Thông báo có thể là thông tin về một giao dịch mới mà client này muốn báo cho các client khác biết về giao dịch mà nó vừa thực hiện.

![03-software_network_talking_transaction.png](/uploads/03-software_network_talking_transaction.png)

Việc chia sẻ thông tin, thông báo lẫn nhau như thế này giúp cho mọi người trên mạng lưới đều cập nhật được các thông tin mới nhất. Điều này khá là quan trọng đối với trường hợp bạn muốn chuyển các loại tiền số ( digital currency ) trên Internet.

![04-software_network_talking_transaction_consensus.png](/uploads/04-software_network_talking_transaction_consensus.png)

> Mạng Bitcoin được mô tả là mạng ngang hàng ( peer to peer network) là vì
>
> 1\. Mọi người đều kết nối với những người tạo thành mạng nên gọi là network.
>
> 2\. Mọi người đều ngang hàng, bình đẳng nên gọi là peer.

**Những ai tạo thành network**

Nhưng đã đề cập ở trên, **bất cứ ai kích hoạt đường truyền Internet và chạy 1 chương trình bitcoin client sẽ là những người tạo nên Bitcoin Network.**

Một cách nghiêm túc, mọi ngươi đều có thể join ( tham gia ) vào mạng Bitcoin.  Tất cả những thứ chúng ta cần chỉ là một đường truyền Internet và phần mềm [Bitcoin Client ](https://bitcoin.org/en/download)

Mỗi lần bạn bật và chạy phần mềm này lên thì máy tính của bạn sẽ trở thành 1 Node trong Bitcoin Network.

![05-nodes_network-0a04fe.png](/uploads/05-nodes_network-0a04fe.png)

**Làm thế nào để join vào mạng Bitcoin**

Download và cài đặt Bitcoin Client. Khi bạn chạy client này thì nó sẽ tự connect với các node khác trên mạng Bitcoin và download một bản sao đầy đủ của blockchain ( file chứa tất các các giao dịch đã được verified ) về máy tính của bạn. Sau đó client sẽ nhận các transaction từ các node khác và đẩy nó luân chuyển trở lại mạng qua các node khác.

Rất có thể bạn phải điều chỉnh một chút cấu hình trên router của mình để có thể cho phép các node khác theo hướng dẫn dưới đây. 

https://bitcoin.org/en/full-node#gui-peer-info

Nhưng đó chỉ là một công việc rất nhỏ thôi.  Chỉ cần download và chạy thì đã hoàn thành 95% chặng đường trở thành 1 active node trên Bitcoin Network rồi.\
\
