Bài 4 stage 6


Phần 1: So sánh hai giải pháp

1. Tiêu chí độ dài:

Cách 1 (Tuyệt đối): Dài dòng, dễ viết sai chính tả.

Cách 2 (Tương đối): Ngắn gọn, súc tích, dễ nhìn.

2. Tiêu chí tính di động (Portability):

Cách 1 (Tuyệt đối): Rất kém. Bị cố định với ổ C: và tài khoản An-K26, gửi cho người khác chạy sẽ bị lỗi FileNotFoundError.

Cách 2 (Tương đối): Rất cao. Chạy được trên mọi máy tính miễn là giữ nguyên cấu trúc thư mục dự án.


Phần 2: Lựa chọn giải pháp tối ưu

Lựa chọn: Em chọn Cách 2 (../data/logs.csv).

Lý do: Đảm bảo tính di động cao nhất, người khác nhận project có thể chạy được ngay mà không cần sửa code.

Ý nghĩa ký hiệu ..: Đại diện cho thư mục cha (lùi ra ngoài 1 cấp thư mục so với vị trí file code đang đứng để trỏ tới thư mục data).
