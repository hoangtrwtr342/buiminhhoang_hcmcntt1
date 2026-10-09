Bài 1 stage 6

Phần 1: Phân tích
1. Không đặt tên thư mục có khoảng trắng trong dấu nháy:
   mkdir Smart Farm Project khiến PowerShell tách Smart, Farm và Project thành các đối số riêng. Vì vậy, lệnh có thể tạo ba thư mục đó thay vì một thư mục tên Smart Farm Project.
   
2. Không đặt đường dẫn có khoảng trắng trong dấu nháy khi dùng cd:
   cd Smart Farm Project truyền nhiều từ vào lệnh, trong khi cd cần một đường dẫn. Hãy viết cd "Smart Farm Project".
   
Lệnh mkdir src/sensors/temperature không sai chỉ vì dùng dấu /: PowerShell hỗ trợ cả / và \ trong đường dẫn

Phần 2: Hoàn thiện
Cách ngắn nhất để tạo toàn bộ cấu trúc trong thư mục hiện tại là:

mkdir "Smart Farm Project\src\sensors\temperature"


Lệnh này tạo thư mục gốc cùng các thư mục lồng nhau. Nếu muốn làm theo từng bước để luyện Tab, hãy tạo thư mục gốc trước, rồi gõ cd "Smart và nhấn Tab để hoàn tất tên thư mục:

mkdir "Smart Farm Project"

cd "Smart Farm Project"

mkdir src\sensors\temperature
