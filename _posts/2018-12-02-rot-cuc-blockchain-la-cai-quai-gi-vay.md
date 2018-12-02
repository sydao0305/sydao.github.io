---
title: Rốt cục blockchain là cái quái gì vậy???
date: 2018-12-02 00:00:00 Z
layout: post
author: Mohit Mamoria
image: https://cdn-images-1.medium.com/max/1600/1*oMwunuVKyqWectTecENigQ.png
excerpt: Giải thích bằng ngôn ngữ vỉa hè dễ hiểu về blockchain.
---

<div class="info">
<h5>Lời người dịch</h5>
<p>Bài viết này của Mohit Mamoria được đăng trên tạp chí <a href="https://hackernoon.com/wtf-is-the-blockchain-1da89ba19348" target="_blank">Hackernoon</a> ngày 30/6/2017. Nhận thấy bài viết vẫn còn rất hữu ích ở hiện tại, cộng tác viên <a href="https://www.facebook.com/nguyet.luu.7509" target="_blank">Spencer Luu</a> đã hiệu đính lại, dựa trên bản dịch của Bùi Quang Tân trên <a href="https://kipalog.com/posts/Blockchain-la-cai-quai-gi-vay---" target="_blank">Kipalog</a>.</p>
</div>

__Trừ khi bạn từ trên trời rơi xuống__ còn không chắc chắn bạn đã từng nghe nói đến Bitcoin và Blockchain.
Đây là 2 từ khóa nổi bật được nhắc đến nhiều trong thời gian qua. Ngay cả anh xe ôm hay bà bán nước cũng bàn tán về nó.

Tôi có nhiều người bạn không làm trong ngành kỹ thuật nhưng vài tuần trở lại đây họ cũng nhờ tôi giải thích về những từ khóa mới này. Tôi đoán có hàng ngàn người ngoài kia cũng cảm thấy như vậy. Và mỗi khi điều đó xảy ra, đấy là cơ hội để viết 1 bài giải ngố, không sử dụng từ ngữ cao siêu, để ai cũng có thể hiểu. Đó là mục đích của bài viết này: để bạn có thể gửi link cho "những tâm hồn lạc lối" kia, mỗi khi họ hỏi “Blockchain là cái &*^% gì?”

### Blockchain - sao lại cần một thứ phức tạp đến vậy?

> For every complex problem there is an answer that is clear, simple, and wrong.
> <cite>H. L. Mencken</cite>

Không giống như những bài viết khác trên internet, thay vì định nghĩa khái niệm blockchain ngay từ đầu, chúng ta sẽ cũng thử tìm hiểu xem vấn đề mà blockchain giải quyết ở đây là gì?

Hãy thử tưởng tượng, Joe là thằng bạn thân của bạn. Nó đi du lịch khắp mọi nơi trên thế giới, bỗng một ngày xấu trời, nó gọi cho bạn "Mày ơi tao đói! Hết cmn tiền rồi :((".

Bạn tỏ ra nhiệt tình "No problem, chờ tao tí".

![Bạn tao đổi với Joe](https://cdn-images-1.medium.com/max/1600/1*BV9t2KZxRV6_ADIsV9OybQ.png)

Rồi gọi cho nhân viên ngân hàng nơi bạn gửi tiền và yêu cầu "Hãy chuyển 1000$ từ tài khoản của tôi sang tài khoản của Joe!".

"Vâng, sếp!"

Nhân viên ngân hàng mở sổ cái, kiểm tra số dư xem bạn có đủ 1000$ hay không.

Bạn là người có tiền mà, nên 1000$ không thành vấn đề. Nhân viên ngân hàng bèn tạo một mục trong cuốn sổ cái, có dạng như sau.

![Nhân viên ngân hàng thêm 1 mục vào sổ cái](https://cdn-images-1.medium.com/max/1600/1*PJ8pYM3jjJAEEkxwOxoRdg.png)

__Lưu ý__ chúng ta sẽ không nhắc đến _máy tính_ để giữ cho mọi thứ đơn giản.
{: .info}

Bạn gọi cho Joe và bảo nó "Ê, tao chuyển tiền rồi đấy. Mày ra ATM mà rút."

![Bạn báo cho Joe là tiền đã chuyển](https://cdn-images-1.medium.com/max/1600/1*nS_5WE-WmhuNioLX8ki4lA.png)

Hãy cùng suy nghĩ xem chuyện gì vừa xảy ra? Cả bạn và Joe đều tin tưởng giao phó cho ngân hàng quản lý tiền của mình. Việc chuyển tiền thực chất chỉ là tạo một chỉ mục trong cuốn sổ cái ở ngân hàng. Hay chính xác hơn, là một chỉ mục trong cuốn sổ mà cả bạn và Joe đều không quản lý hay sở hữu.

Và đó chính là vấn đề của các hệ thống đang tồn tại.

Để tạo dựng niềm tin giữa các cá nhân, chúng ta đang phải dựa vào một bên thứ ba.
{: .non-quote}

Trong nhiều năm qua, chúng ta đều phải phụ thuộc vào những bên trung gian để có thể tin tưởng lẫn nhau. Vậy, phụ thuộc vào họ thì có vấn đề gì?

- Điều gì sẽ xảy ra nếu cuốn sổ cái lưu trữ những giao dịch của bạn bị hack, bị xóa?
- Sẽ thế nào nếu giả sử giao dịch của bạn bị người ta nhập lỗi, bạn bị chuyển khoản 1500$ thay vì 1000?
- Hay sẽ thế nào nếu nhân viên ngân hàng tự ý thực hiện những giao dịch ý đồ không trong sáng?

Trong suốt nhiều năm qua, chúng ta đều đã đặt tất cả số trứng mình có vào một giỏ, và thậm chí nó còn chẳng phải là cái giỏ của mình.
{: .non-quote}

Vậy liệu có thể có một hệ thống mà chúng ta có thể dùng để chuyển tiền mà không cần nhờ đến ngân hàng không?

Để trả lời câu hỏi này, chúng ta cần phải đào sâu hơn nữa, và đặt ra một câu hỏi tốt hơn (sau tất cả, chỉ có những câu hỏi hay ho mới dẫn đến những câu trả lời xuất sắc).

Hãy thử suy nghĩ một chút, khái niệm "chuyển tiền" thực ra nghĩa là gì? Đối với ngân hàng, đó chỉ là một chỉ mục trong cuốn sổ cái phải không? Vậy thì câu hỏi cần đặt ra là:

__Liệu có cách nào để duy trì nội dung của cuốn sổ cái giữa chúng ta thay vì phải nhờ đến ai khác làm hộ việc đó?__

Đó là một câu hỏi đáng giá. Hiển nhiên bạn hoàn toàn có thể đoán ra được câu trả lời. Đó chính là blockchain.

Blockchain là một phương thức để duy trì cuốn sổ cái giữa tất cả các người dùng, thay vì phải thông qua bên thứ 3 khác.

Bạn vẫn tiếp tục đọc đến đây chứ? Thật tuyệt, bởi vì ngay từ lúc này, sẽ có rất nhiều câu hỏi nảy ra trong đầu bạn, và chúng ta sẽ cùng nhau tìm hiểu hệ thống sổ cái phân tán (distributed ledger) này hoạt động như thế nào nhé.

### Ok, thế tóm lại nó hoạt động như nào?

Yêu cầu chính của phương thức này là phải có đủ số lượng người cần thiết, những người không muốn tiền của họ phụ thuộc vào bên thứ ba. Chỉ có như vậy nhóm người này mới có thể tự duy trì được sổ cái của họ.

Một câu hỏi đặt ra là bao nhiêu người thì được coi là đủ? Càng nhiều càng tốt. Ít nhất là 3.

Trong ví dụ sau đây, giả sử có 10 người. Theo thỏa thuận, mỗi người sẽ có thông tin chi tiết về danh sách giao dịch của những người khác, nhưng không cần biết danh tính (tức là, không biết giao dịch đã cho là ông Nguyễn Văn Đốp gửi cho bà Lê Thị Chát).

![10 nguòi đồng ý tham gia hệ thống](https://cdn-images-1.medium.com/max/1600/1*0uFEch5XGG_Gqex1wXTFWg.png)

#### 1. Chuẩn bị

Tất cả mọi người đều được cung cấp: 1 thư mục _rỗng_ để đựng tài liệu, 1 tập giấy _trắng_, và 1 chiệc bút chì. Giờ thì bắt đầu thôi.

#### 2. Giao dịch đầu tiên

Giả sử có một giao dịch xảy ra, #2 muốn chuyển 10$ cho #9.

Để thực hiện giao dịch, #2 thông báo với tất cả mọi người "Tôi muốn chuyển 10$ cho #9. Mọi người xin hãy ghi lại vào trang giấy của mình".

![#2 thông báo muốn chuyển tiền](https://cdn-images-1.medium.com/max/1600/1*IJPEjo45XSbkB7nGA854FQ.png)

Tất cả mọi người liền cùng kiểm tra xem #2 có đủ số dư trong tài khoản để chuyển 10$ hay không. Nếu OK, tất cả sẽ cùng ghi lại thông tin giao dịch vào trang giấy của mình.

![Giao dịch được ghi vào trang giấy](https://cdn-images-1.medium.com/max/1600/1*m0lFIWh2bmurf_6rPXoozw.png)

Giao dịch khi đó được coi là hoàn thành.

#### 3. Các giao dịch tiếp theo

Theo thời gian, ngày càng có nhiều người trong hệ thống có nhu cầu chuyển tiền cho nhau. Cứ mỗi khi muốn thực hiện một giao dịch, họ sẽ thông báo với tất cả những người khác. Và ngay khi nghe thấy thông báo, những người còn lại sẽ kiểm tra rồi viết thông tin giao dịch đó vào trang giấy của mình.

Chẳng bao lâu sau, trang giấy của mọi người đều đã kín. Đã đến lúc phải cất trang giấy đó vào thư mục và lấy ra trang giấy trắng mới để tiếp tục làm việc.

#### 4. Niêm phong trang giấy

Trước khi cất, chúng ta cần niêm phong trang giấy bằng một con dấu mà tất cả mọi người trong hệ thống đều đồng ý và xác minh được. Bằng cách đó, chúng ta sẽ đảm bảo rằng mãi mãi không ai có thể thay đổi được nội dụng của trang giấy đó nữa. Trang giấy ở trong thư mục riêng của một người cần phải giống hệt trang tương ứng ở thư mục của những người khác. Giống cả về nội dung lẫn dấu niêm phong.

Một khi đã ở trong thư mục, nó sẽ mãi ở trong đó, và luôn được niêm phong. Hơn nữa, vì mọi người tin tưởng vào dấu niêm phong, họ sẽ tin tưởng vào nội dung của trang giấy. Dấu niêm phong chính là điểm mấu chốt của phương pháp này.

Quá trình niêm phong này được gọi là "đào" (mining).
{: .info}

Trước kia, các bên trung gian thứ 3 (ngân hàng, các tổ chức tài chính) tạo cho chúng ta niềm tin rằng bất cứ điều gì họ viết trong cuốn sổ cái sẽ không bao giờ thay đổi. Trong một hệ thống phân tán (distributed) và phi tập trung (decentralized) như hệ thống tôi đang mô tả, dấu niêm phong sẽ cung cấp niềm tin tương tự như thế.
{: .non-quote}

### Thật thú vị! Vậy chúng ta sẽ niêm phong như thế nào?

Trước khi tìm hiểu xem làm thế nào để có thể niêm phong lại trang giấy, chúng ta cần phải hiểu cách thức hoạt động của dấu niêm phong một cách tổng quát.

Đã đến lúc chúng ta cùng làm quen với một thứ được gọi là...

#### Cỗ máy thần kỳ

Hãy tưởng tượng có một cỗ máy được bao quanh bởi các bức tường dày. Nếu bạn đưa vào cỗ máy này một chiếc hộp chứa bên trong một thứ gì đó từ phía bên trái, nó sẽ trả ra một chiếc hộp chứa một thứ gì đó khác.

Cỗ máy này có tên thật là Hash Function (Hàm băm). Nhưng để cho đơn giản, hãy gọi nó là Cỗ máy thần kỳ.
{: .info}

![Cỗ máy thần kỳ](https://cdn-images-1.medium.com/max/1600/1*ox9O7DmN1I1AiyNygulCrw.png)

Giả sử thế này, bạn gửi vào cỗ máy số `4` từ bên trái, sau quá trình xử lý nó sẽ đưa trả lại bạn một chuỗi ký tự `dcbea` ở bên phải.

![hash(4) == dcbea](https://cdn-images-1.medium.com/max/1600/1*G9UsASIX8eX_3xU1_3pg-w.png)

Làm thế nào cỗ máy này có thể chuyển đổi từ số `4` sang xâu ký tự kia? Không ai biết. Hơn nữa, đây là một quá trình không thể đảo ngược, nghĩa là bạn KHÔNG thể gửi vào máy xâu ký tự `dcbea` và nhận lại giá trị ban đầu là số `4`. Nhưng bất cứ khi nào bạn đưa số `4` vào cỗ máy này, nó đều sẽ trả về cho bạn cùng một xâu ký tự là `dcbea`.

Bây giờ hãy thử gửi một con số khác vào máy nhé. `26` thì sao?

![hash(26) == 94c8e](https://cdn-images-1.medium.com/max/1600/1*HR3OyX1P-eeiwaOalY-W5A.png)

Lần này chúng ta nhận được chuỗi `94c8e`, và hãy để ý, chuỗi kết quả trả về có thể chứa ký tự là chữ số.

Bây giờ tôi muốn hỏi bạn câu hỏi này:

__Bạn có thể nói cho tôi biết tôi cần gửi vào máy con số nào từ bên trái để có thể nhận được một chuỗi ký tự mà bắt đầu bằng 3 chữ số 0 không? VD: `000ab`, `00069` hoặc `000fa`, v.v.__

![Thử dự đoán đầu vào](https://cdn-images-1.medium.com/max/1600/1*1p-LJxci-vdJ7JObPDcaUg.png)

Hãy thử suy nghĩ 1 chút về câu hỏi này.

Như tôi đã nói với các bạn, rằng với chuỗi ký tự được trả về ở bên phải, cỗ máy thần kỳ này không thể cho chúng ta biết giá trị đầu vào ở bên trái là gì. Vậy làm thế nào có thể trả lời được câu hỏi trên?

Tôi có nghĩ đến một phương pháp. Đó là sao chúng ta không lần lượt thử từng số một từ 0 đến vô cùng, cho đến khi thu được kết quả thoả mãn?

![Cứ thử lần lượt từng số một](https://cdn-images-1.medium.com/max/1600/1*NanhTPqi85WkwQoEpGQGHw.png)

Hãy lạc quan lên, sau vài nghìn lần thử, biết đâu chúng ta sẽ tìm được chuỗi ký tự đáp ứng yêu cầu (đầu với 3 chữ số 0)!

![Đã tìm được số đầu vào](https://cdn-images-1.medium.com/max/1600/1*_BOLJbfmKu8U1LNTtS_UMw.png)

Bạn thấy đấy, việc từ đầu ra tính ngược để tìm đầu vào là vô cùng khó khăn. Nhưng đồng thời, lại rất dễ dàng để kiểm tra xem một đầu vào có ứng với đầu ra cho trước hay không. Nhớ rằng nếu cho cùng 1 giá trị đầu vào vào thì lần nào cỗ máy này cũng cho ra giá trị đầu ra như nhau.

Giờ nghĩ xem, nếu tôi đưa bạn một số, chẳng hạn `72533`, và hỏi bạn "Số này nếu đưa vào máy thì có thể cho ra một chuỗi ký tự bắt đầu bằng 3 chữ số 0 hay không?"

Tất cả những gì bạn cần làm là ném con số này vào cỗ máy thần kỳ và kiểm tra kết quả đầu ra. Chỉ chạy thử thì mới biết, không có cách nào đoán được.

Đó cũng chính là chức năng quan trọng nhất của cỗ máy này.

Với một kết quả đầu ra cho trước, sẽ hầu như không thể truy ngược lại giá trị đầu vào. Nhưng nếu đã có cả giá trị đầu ra và đầu vào, bạn sẽ dễ dàng xác minh được chúng có phải là "1 cặp" hay không. Chỉ cần ném đầu vào vào máy, và so sánh đầu ra.
{: .non-quote}

#### Sử dụng cỗ máy này để niêm phong như thế nào?

Chúng ta sẽ cùng sử dụng cỗ máy thần kỳ này để sinh ra một dấu niêm phong cho những trang giấy. Như mọi khi, chúng ta sẽ cùng bắt đầu với một tình huống giả định.

Hãy tưởng tượng tôi đưa cho bạn 2 chiếc hộp. Chiếc hộp đầu tiên chứa con số `20893`. Sau đó, tôi sẽ hỏi bạn "Ê, cậu tìm cho tôi một số mà khi cộng với con số trong chiếc hộp đầu tiên rồi đưa vào cỗ máy thần kỳ thì sẽ trả ra một chuỗi ký tự bắt đầu bằng 3 chữ số 0."

![Làm sao tìm được số đó?](https://cdn-images-1.medium.com/max/1600/1*0ChKQgKuRoOoFtj_jTMx2g.png)

Tình huống này tương tự những ví dụ ở phần trước. Cách duy nhất để tính toán ra con số cần tìm là lần lượt thử tất cả các số hợp lệ từ 0 đến vô cùng.

Giả sử, sau vài nghìn lần thử, chúng ta ngẫu nhiên bắt được con số đó, là số `21191`. `20893` + `21191` = `42084`. Đưa qua cỗ máy, nó trả về chuỗi ký tự bắt đầu bằng 3 số 0 là `00078`.

![Đã tìm ra](https://cdn-images-1.medium.com/max/1600/1*ewcdx7L6_D1RIvbPFrMYiw.png)

Trong trường hợp này, con số `21191` được gọi là dấu niêm phong cho số `20893`.

Giả sử nội dung trang giấy cần niêm phong được đại diện bằng con số `20893`. Để niêm phong nó, chúng ta dùng 1 con dấu khắc số `21191` và dóng dấu lên trên trang giấy. Ngay khi được đóng giấu, trang giấy được coi là đã bị niêm phong và có thể được đưa vào thư mục.

![Đã niêm phong](https://cdn-images-1.medium.com/max/1600/1*W5XSeKP6xoAQbxmmW4-dog.png)

Con số niêm phong được gọi là Proof of Work (PoW). Có nghĩa nó là bằng chứng cho công sức tính toán ra nó (công sức thử lần lượt các số cho đến khi tìm ra số thoả mãn). Ở bài viết này, chúng ta vẫn sẽ thống nhất gọi nó là số niêm phong nhé.
{: .info}

Nếu ai đó muốn xác nhận xem nội dung của trang có bị thay đổi sau khi đã niêm phong không, tất cả những gì anh ta cần làm là cộng nội dung của trang với số niêm phong và đưa qua cỗ máy thần kỳ.

Nếu cỗ máy trả về một chuỗi ký tự bắt đầu bằng 3 chữ số 0, có nghĩa nội dung của trang không hề bị thay đổi. Nếu ngược lại, chúng ta có thể vứt bỏ trang giấy đó đi vì nó đã bị ai đó sửa vào và không còn hợp lệ.

Chúng ta sẽ sử dụng cơ chế này để niêm phong tất cả các trang trước khi sắp xếp chúng trong thư mục.

#### Ai là người niêm phong?

Để niêm phong trang giấy ghi các thông tin giao dịch của bộ hệ thống, chúng ta cần tìm ra một con số mà khi nối vào danh sách giao dịch và đưa qua cỗ máy thần kỳ, chúng ta sẽ thu được một chuỗi ký tự bắt đầu bằng 3 chữ số 0.

![Tìm số niêm phong cả trang giấy](https://cdn-images-1.medium.com/max/1600/1*ijsTUoELxn6zFkBa7r23VA.png)

__Lưu ý__ tôi hay sử dụng cụm từ "chuỗi ký tự bắt đầu bằng 3 chữ số 0" chỉ như là một ví dụ đơn giản. Mục đích là để minh hoạ cỗ máy thần kỳ hoạt động như thế nào. Câu đố được dùng trong thực tế phức tạp hơn rất nhiều, không đơn giản là 3 số 0.
{: .info}

Một khi đã bỏ ra thời gian (và điện năng) để tính ra số niêm phong, nó sẽ được dùng để niêm phong trang thông tin giao dịch. Nếu có một ai đó thử thay đổi nội dung của trang giấy này, số niêm phong sẽ cho phép bất kỳ ai cũng có thể kiểm tra và phát giác.

Sau khi đã hiểu về cơ chế niêm phong, chúng ta sẽ cùng quay lại thời điểm khi trang ghi đã kín và hết chỗ để viết thêm.

Lúc này, tất cả mọi người trong mạng sẽ cùng thực hiện việc tính toán để tìm ra con số niêm phong. __Người đầu tiên__ tìm ra được số niêm phong sẽ thông báo cho tất cả những người còn lại.

![Người đầu tiên tìm thấy](https://cdn-images-1.medium.com/max/1600/1*oMwunuVKyqWectTecENigQ.png)

Ngay khi nhận được số niêm phong, tất cả mọi người trong mạng sẽ xác nhận xem nếu dùng cỗ máy thần kỳ với đầu vào là số niêm phong và trang ghi thông tin giao dịch, chuỗi ký tự trả về có thoả mãn yêu cầu đưa ra hay không. Nếu có, từng người sẽ đóng dấu trang thông tin giao dịch của mình với số niêm phong này và đặt nó vào thư mục của mình.

Nhưng nếu có ai đó, giả sử là #7, nói rằng số niêm phong này không thoả mãn yêu cầu đầu ra. Những trường hợp như vậy không phải là điều bất thường.

Những lý do có thể gây ra điều này bao gồm:

- Có lỗi nào đó trong quá trình tiếp nhận thông tin, do đó số niêm phong #7 nhận được không phải là số niêm phong đã được thông báo ra
- Anh ta có thể đã sai sót khi xử lý thông tin nhận được
- Anh ta có thể đã cố gắng lừa dối mọi người vì động cơ nào đó

Không quan trọng lý do là gì, #7 chỉ có duy nhất một lựa chọn: bỏ trang ghi thông tin giao dịch của mình đi, rồi copy trang đã được niêm phong từ hàng xóm, sau đó đặt nó vào tập thư mục của mình.

Nếu #7 không đưa trang nào vào thư mục, anh ta không thể tiếp tục viết thêm các giao dịch mới nữa, và như vậy anh ta sẽ không thể tiếp tục tham gia cuộc chơi. Mọi người đều đã sang trang tiếp theo mất rồi!

Số niêm phong nào được đa số thành viên trong mạng chấp thuận sẽ trở thành số niêm phong chính thức được sử dụng.
{: .non-quote}

__Một câu hỏi được đặt ra là, vậy tại sao tất cả mọi người lại phải bỏ công sức, nguồn lực của mình để thực hiện việc tính toán số niêm phong. Tại sao không đơn giản chỉ cần ngồi đợi người khác tính và thông báo cho mình?__

Đây là một câu hỏi tuyệt vời. Ai cũng ngồi đợi thì hệ thống không thể hoạt động. Chúng ta cần phần thưởng! Tất cả mọi người là thành viên của mạng Blockchain đều có đủ tiêu chuẩn tham gia tìm số niêm phong để nhận phần thưởng. Người đầu tiên tìm ra được số niêm phong sẽ nhận được phần thưởng, dành cho công sức anh ta đã bỏ ra (tiền máy móc, tiền điện, v.v.).

Hãy tưởng tượng đơn giản thế này, nếu #5 tìm ra số niêm phong của một trang, anh ta sẽ nhận được phần thưởng là một khoản tiền. Tài khoản của #5 được cộng thêm, nhưng không có ai trong hệ thống phải chuyển tiền cho #5. Tiền thưởng được hệ thống "in" ra để thưởng, vì vậy mà gọi là "đào" - đào được tiền thưởng (vàng) từ lòng đất.

Đó chính là cách Bitcoin ra đời. Đó là loại tiền tệ đầu tiên được giao dịch trên Blockchain (sổ cái phân tán). Các thành viên nỗ lực tính toán "số niêm phong" để giữ cho hệ thống chạy. Đổi lại, họ được trả thưởng bằng chính những đồng bitcoin.

Tiền thưởng chính là thứ thúc đẩy mọi người làm việc, và vì thế hệ thống được duy trì.
{: .non-quote}

Và mỗi khi mọi người cất trang giấy đã ghi kín thông tin giao dịch của mình vào thư mục, họ lại tiếp tục lấy ra một trang giấy mới ra, và lặp lại toàn bộ quá trình này - cứ như vậy.

Một trang giấy chính là 1 Khối (Block) giao dịch, và thư mục chính là một Chuỗi các Khối (Chain of Block). Giờ thì bạn đã hiểu vì sao gọi là "blockchain" rồi nhé!
{: .info}

<div class="line"></div>

__À, còn một điều nữa__ tôi quên chưa nói cho bạn biết.

Hãy tưởng tượng giả sử trong tập tài liệu đã có 5 trang ghi kín các thông tin giao dịch - và tất cả đều đã được đóng dấu niêm phong. Điều gì sẽ xảy ra nếu tôi quay lại trang thứ 2 và sửa thông tin một vài giao dịch để làm lợi cho bản thân mình.

Như chúng ta đã cùng thảo luận trước đó, số niêm phong sẽ cho phép mọi người phát hiện ra sự thay đổi trong các giao dịch đã niêm phong đúng không? Nhưng nếu tôi sửa giao dịch, sau đó tính toán lại số niêm phong rồi đóng dấu lại thì sao?

Để ngăn chặn việc này, người ta đưa ra một số quy định cho việc cho tính toán số niêm phong.

### Chống thay đổi số niêm phong của trang trong quá khứ

Bạn có nhớ lúc trước tôi đã bảo là đưa cho bạn 2 chiếc hộp không? Một chiếc hộp chứa con số `20893`, chiếc còn lại để trống để chứa con số bạn sẽ tính toán. Trong thực tế, để tính toán một số niêm phong trong một Blockchain, thay vì 2, hệ thống sẽ cung cấp cho bạn 3 hộp - 2 hộp đã được điền sẵn và một hộp trống để dành cho bạn.

Sẽ phải ghép cả 3 hộp này lại để đưa vào cỗ máy thần kỳ tìm số niêm phong.

Chúng ta đã biết rằng một hộp chứa danh sách các giao dịch, một hộp thì chứa số niêm phong. Vậy hộp thứ 3 chứa gì?
Hộp thứ 3 sẽ chứa số niêm phong của trang giao dịch trước.

![Có 3 hộp chứ không phải 2](https://cdn-images-1.medium.com/max/1600/1*Vz0UOPPuWYz8YNRhy0NCNQ.png)

Với thủ thuật nhỏ này, chúng ta có thể đảm bảo rằng bất kỳ trang giao dịch nào đều phụ thuộc vào trang trước đó. Do đó, nếu ai đó có ý định thay đổi một trang trong quá khứ, ngoài việc số niêm phong ở trang đó bị sai thì tất cả các số niêm phong ở các trang sau đó cũng bị sai. Anh ta sẽ phải niêm phong lại tất cả các trang sau đó, để giữ cho tập tài liệu của mình được hợp lệ.

Chúng ta đã biết, việc tính toán ra số niêm phong mất thời gian (và năng lượng) thế nào. Nếu 1 người gian dối muốn sửa quá khứ, anh ta sẽ không thể nào niêm phong thư mục của mình kịp tiến độ với 9 người còn lại.

Theo quy định, chuỗi dài nhất (thư mục chứa nhiều trang giấy nhất) là trung thực.
{: .non-quote}

![Chuỗi dài nhất là trung thực](https://cdn-images-1.medium.com/max/2000/1*CRmIEzvK0k1fM--onASiHQ.png)

Ở hình trên, chuỗi đóng dấu đỏ là dài nhất, nên nó được coi là trung thực.

Thành ra, 1 gã không trung thực sẽ không thể đánh bại 9 người trung thực còn lại, chỉ lãng phí công sức tiền của mà thôi.

Khi tôi nói vậy, có điều gì đó nảy ra trong đầu bạn không?

### Điều gì xảy ra nếu, thay vì 1, mà là 6 người trong mạng cùng trở nên không trung thực?

Trong trường hợp này, những người khác không còn có thể tin vào hệ thống nữa. Nếu tiếp tục tham gia, họ có khả năng bị mất tiền. Vấn đề này được gọi là [51% Attack](/blog/2018/11/26/tan-cong-51-la-gi.html). Nếu phần lớn các thành viên trong mạng quyết định gian lận để lừa dối những người còn lại, hệ thống sẽ không còn bảo vệ được các thành viên trung thực.

Và đó là lý do duy nhất để Blockchain có thể sụp đổ, nếu có lúc nào đó nó sụp đổ. Có thể chúng ta tin tưởng rằng điều này khó có thể xảy ra, nhưng dù sao vẫn cần phải biết điểm yếu của hệ thống. Blockchain được xây dựng trên giả định rằng đa số đám đông luôn luôn là trung thực.

Xong rồi đấy. Tóm lại là blockchain nó hoạt động như vậy. Bây giờ, nếu có ai hỏi bạn "Blockchain là cái &*^% gì?" thì chỉ cần gửi link bài viết này cho họ là xong.

Bạn có nghĩ ra ai cần đọc bài này? Hãy share lại cho họ luôn.