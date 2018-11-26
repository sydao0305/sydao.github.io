---
title: Tấn công 51% là gì?
image: /assets/img/hashrate.jpg
excerpt: 51% của cái gì và gây hại như thế nào.
---

Giá trị của blockchain nằm ở chỗ nó loại bỏ sự độc quyền trong việc _thay đổi_ dữ liệu chung. Tuy nhiên, khi có 1 đối tượng hoặc 1 nhóm đối tượng liên kết với nhau để chiếm hơn 50% quyền thay đổi dữ liệu thì sự dân chủ - giá trị cốt lõi của blockchain - bị lung lay tận gốc rễ.

Khái niệm “tấn công 51%” thường được dùng cho các hệ thống:
- Cấu trúc dữ liệu được sử dụng là blockchain (không phải các cấu trúc hiếm dùng như Tangle, vv.)
- Thuật toán đồng thuận là Proof of Work (tức là cơ chế đào - mining)

Các hệ thống dùng cấu trúc dữ liệu hoặc thuật toán đồng thuận khác cũng có rủi ro bị tấn công tương tự. Tuy nhiên khi ấy, con số % cùng ý nghĩa và cách thức thực hiện sẽ khác đi.

Cả Bitcoin và Ethereum, 2 blockchain lớn nhất hiện nay, đều thoả mãn 2 điều kiện trên, nên đều là đối tượng của tấn công 51%. Con số 51% được chọn để đặt tên cho gọn, hàm ý là “lớn hơn 50%”.

### 51% của cái gì?

Các máy tính tham gia vào mạng lưới blockchain gọi là các node. Một số node bật chế độ đào, gọi là máy đào.

Nhiệm vụ của các máy đào là sẽ phải tìm ra 1 con số, gọi là giá trị băm (hash), thoả mãn điều kiện đã cho. Ai tìm ra sớm nhất sẽ được quyền thêm block mới vào blockchain và nhận tiền thưởng.

Khốn nỗi, bạn không thể đoán trước được giá trị hash, bạn phải tính toán ra nó rồi mới biết nó có “trúng giải” không. Vì vậy, các máy đào phải có năng lực tạo hash mới càng nhanh càng tốt, hòng tìm ra hash trúng giải sớm hơn các máy đào khác.

Tổng số lượng giá trị hash mà toàn bộ mạng lưới máy đào tạo ra trong 1 đơn vị thời gian gọi là _hash rate_.

Chiếm 51% tức là chiếm 51% hash rate. Đồng nghĩa, về mặt _xác xuất_, có 51% khả năng chiến thắng ở mỗi vòng thi.

<div class="media">
  <img src="/assets/img/hashrate.jpg">
  <p class="caption">Thị phần hash rate giữa các xưởng đào lớn trong 24h ngày 26/11/2018 - theo <a href="https://www.blockchain.com/en/pools" target="_blank">Blockchain.info</a></p>
</div>

### Chiếm 51% vẫn KHÔNG làm được gì?

51% thì cũng không thể thay đổi nội dung các giao dịch. Các máy đào chỉ có thể xác nhận các giao dịch có hợp lệ hay không, rồi thực hiện sắp xếp giao dịch vào block để “đào”.

51% thì cũng không thể tạo ra các giao dịch không hợp lệ. Chẳng hạn, tiêu tiền quá số dư hoặc tiêu tiền của người khác. Các node trong mạng lưới sẽ kiểm tra và từ chối các giao dịch như vậy.

Cũng không khả thi nếu họ muốn thay đổi cách sắp xếp giao dịch ở các block sâu trong quá khứ. Vì khi đó sẽ phải đào lại tất cả block xảy ra sau đó. Mà thời gian đào mỗi block khá là lâu (đối với bitcoin là 10 phút, Ethereum là 17 giây, nếu đào lại 1 mình thì còn lâu hơn). Do đó, để đào kịp tiến độ với phần còn lại thì mất rất nhiều thời gian và chi phí - thường lớn hơn nhiều so với tiền kiếm được (nếu có).

## Chiếm 51% có thể làm gì?

Thứ nhất, họ có thể “kiểm duyệt” giao dịch vì lý do không lành mạnh. Chẳng hạn, không sắp xếp vào block tấcácả giao dịch gửi đến địa chỉ của Amazon. Điều này thì không cần chiếm 51%, cứ có số % lớn đủ gây ảnh hưởng là có thể làm được.

Thứ hai, họ có thể tiêu 1 khoản tiền 2 lần (double spending).

Để hiểu được vì sao, cần biết thêm về cách thức phối hợp giữa các máy đào. Mỗi khi đào được 1 block hợp lệ, máy đào ngay lập tức phát tán đi khắp mạng lưới. Các máy đào khác khi nhận được sẽ xác nhận, lưu lại, rồi chuyển sang đào block tiếp theo.

Bởi vì đường truyền có độ trễ nên khi bạn đào được 1 block thì cũng mất mấy giây mới truyền tới máy đào khác cách nửa vòng trái đất. Điều ghì xảy ra khi trong thời gian đó máy bên kia cũng đào được? Khi đó xảy ra hiện tượng fork tạm thời: blockchain lưu ở 1 số node có sự khác biệt so với blockchain lưu ở các node còn lại.

Để giải quyết, 1 quy định được đưa ra: bên nào dài hơn bên ấy hợp lệ. Ban đầu thì độ dài của blockchain ở 2 nhánh là bằng nhau. Tuy nhiên, sau một thời gian, nhánh nào được đào bởi tập hợp máy đào có hash rate lớn hơn sẽ dài hơn. Khi đó, các node sẽ đồng loạt chuyển sang dùng bản dài hơn, và nhánh ngắn hơn không còn ý nghĩa. Sẽ chẳng còn máy đào nào phí công đào cái nhánh bỏ đi đó nữa.

Đối tượng máy đào chiếm 51% hash rate có thể tiêu 1 khoản tiền 2 lần theo cách như sau:

- Thực hiện 1 giao dịch chuyển tiền để mua 1 xe máy điện Clara, tạm gọi là _giao dịch A_
- Âm thầm thực hiện đào các block, nhưng cố tình bỏ qua giao dịch A kia. Đào được 1 block thì không truyền cho các máy đào khác mà âm thầm đào tiếp trong bóng tối. Ta tạm gọi là _nhánh tối_
- Ở nhánh sáng, các máy đào khác xác nhận giao dịch A. Phía cửa hàng sau khi thấy giao dịch thành công, đợi 1 thời gian ngắn cho block đủ sâu, rồi giao hàng
- Lúc này, nhánh tối đã dài hơn nhánh sáng. Sau khi nhận được xe Clara, đối tượng mới thực hiện phát tán nhánh tối ra mạng lưới. Các node đồng loạt chấp nhận nhánh tối, do nó dài hơn. Trong nhánh tối không có giao dịch A, nên tiền vẫn còn trong tài khoản. Trong khi hàng thì đã nhận rồi!

<div class="media">
  <img src="/assets/img/attack51.jpg">
  <p class="caption">Áo đỏ chiếm 51% âm thầm đào rồi phát tán khi đã dài hơn nhánh chính</p>
</div>

Như vậy là đối tượng có xe Clara đi mà không mất tiền, sau đó lại dùng tiền đó để tiêu tiếp. Mặc dù cửa hàng đã đợi cho block được xác nhận đủ lâu mới giao hàng nhưng vẫn không tránh được cú lừa này.

Hơn nữa, do đào nhánh tối hoàn toàn một mình, đối tượng chiếm toàn bộ tiền thưởng!

Về mặt lý thuyết, nếu có đủ sức mạnh, có thể kiên nhẫn đào lại toàn bộ block trong quá khứ để nhận hết phần thưởng. Tuy nhiên, làm như vậy giá trị của đồng coin tương ứng sẽ rớt thảm, tiền thưởng đó sẽ không thấm vào đâu so với chi phí đào.

Trên thực tế, tấn công 51% chưa xảy ra lần nào với Bitcoin và Ethereum. Vào năm 2014, ghash.io có lúc vượt 50% hash rate của Bitcoin. Tuy nhiên, sau đó nó tự nguyện giảm xuống và hứa sẽ không bao giờ vượt quá 40%, vì sự lành mạnh của mạng lưới là một đảm bảo về quyền lợi của máy đào. Các blockchain nhỏ hơn thì không được may mắn như thế. Do chi phí để chiếm phần lớn hash rate không quá lớn, đã có nhiều cuộc tấn công 51% được ghi nhận (như đối với Bitcoin Gold, Verge, v.v.).

Chiếm 51% hash rate còn có thể làm được 1 số điều khác, nhưng 2 điều đã nói ở trên là cơ bản nhất.