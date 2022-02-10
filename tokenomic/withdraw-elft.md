# Rút Token ELFT

Hệ thống rút Token hoạt động riêng biệt trên từng tài khoản. Mỗi tài khoản sẽ có mức phí giao dịch khác nhau. Mức phí giao dịch dựa vào thời gian giữa các lần rút.

Phí rút Token bắt đầu từ 75% khối lượng giao dịch. Sau mỗi ngày, phí rút Token sẽ giảm đi 5%, phí rút Token tối thiểu là 5%. 60% phí rút Token sẽ bị tiêu hủy để thúc đẩy giá trị Token.

Sau đây là phí rút Token:

| Thời gian rút Token (Ngày) | Phí rút Token |
| -------------------------- | ------------- |
| 0                          | 75%           |
| 1                          | 70%           |
| 2                          | 65%           |
| 3                          | 60%           |
| 4                          | 55%           |
| 5                          | 50%           |
| 6                          | 45%           |
| 7                          | 40%           |
| 8                          | 35%           |
| 9                          | 30%           |
| 10                         | 25%           |
| 11                         | 20%           |
| 12                         | 15%           |
| 13                         | 10%           |
| 14                         | 5%            |

Sau mỗi lần hoàn tất rút Token, bộ đếm sẽ được reset.

_Ví dụ:_

* _Trường hợp **** 1: Rút 100 ELFT, nếu là ngày thứ 3 kể từ lần cuối rút Token, phí rút là 60%. Người dung sẽ nhận được 40 ELFT. Thanh toán 60 ELFT (100\*60%) là phí thủ tục, trong đó có 36 ELFT (60\*60%) sẽ bị tiêu hủy._
* _Trường hợp 2: Rút 100 ELFT, nếu là ngày thứ 14 kể từ lần cuối rút Token, phí rút sẽ là **thấp nhất 5%.** Nhận được 95 ELFT. Thanh toán 5 ELFT（100\*5%）là phí thủ tục, trong đó có 3 ELFT (5\*60%) sẽ bị tiêu hủy._
