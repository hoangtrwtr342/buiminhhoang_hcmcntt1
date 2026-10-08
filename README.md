Bài4 Stage 5

Phần 1: Phân tích & So sánh (Ưu / Nhược điểm)

Em xin phân tích và so sánh hai cách viết đường dẫn dựa trên 3 tiêu chí:

1. Về tính di động (Portability):

Cách 1 (Tuyệt đối): Rất kém. Đường dẫn bị gán cứng (hard-code) với ổ C: và tài khoản An. Khi gửi cho bạn bè (khác tên User hoặc khác ổ đĩa), code sẽ báo lỗi FileNotFoundError ngay lập tức.
Cách 2 (Tương đối): Rất cao. Không phụ thuộc vào tên người dùng hay phân vùng ổ đĩa. Chỉ cần giữ nguyên cấu trúc thư mục dự án, code có thể chạy trên mọi máy tính (Windows, macOS, Linux).

2. Về độ dài câu lệnh:

Cách 1 (Tuyệt đối): Dài dòng, rườm rà, dễ gõ sai chính tả và khó bảo trì khi cấu trúc thư mục thay đổi.
Cách 2 (Tương đối): Ngắn gọn, súc tích, trực quan và dễ đọc hiểu.

3. Về tính an toàn:

Cách 1 (Tuyệt đối): Kém an toàn vì làm lộ tên tài khoản cá nhân (An) và cấu trúc ổ đĩa thật của máy tính khi chia sẻ mã nguồn.
Cách 2 (Tương đối): An toàn hơn vì chỉ để lộ cấu trúc nội bộ của dự án, bảo mật được thông tin môi trường hệ thống.
Phần 2: Lựa chọn giải pháp tối ưu

1. Chốt giải pháp:

Em chọn Cách 2 (Đường dẫn tương đối: ../Data/users.csv).
Lý do: Đáp ứng chính xác quy tắc nghiệp vụ: chương trình vẫn chạy được khi gửi toàn bộ thư mục Project cho bạn bè (dù khác tên User hay khác ổ đĩa).

2. Giải thích ý nghĩa của các ký hiệu . và ..:

Ký hiệu . (Một dấu chấm): Đại diện cho thư mục hiện tại nơi mã nguồn hoặc terminal đang đứng.
Ký hiệu .. (Hai dấu chấm): Đại diện cho thư mục cha (lùi ra ngoài 1 cấp so với vị trí hiện tại).
Cơ chế hoạt động: Đoạn code đang nằm trong thư mục src:
.. sẽ lùi ra ngoài 1 cấp để về thư mục gốc Project.
Tiếp tục trỏ vào Data/users.csv để mở đúng tệp dữ liệu.
