Bài 3 stage 6

1. tạo thư mục bằng một dòng lệnh

- New-Item -ItemType Directory -Force -Path "smart-farm\data\logs", "smart-farm\code", "smart-farm\backup"

2.tạo file bằng một dòng lệnh

-New-Item -ItemType File -Path "smart-farm\code\config.json", "smart-farm\code\sensors.py", "smart-farm\code\.env"

3. Sao chép toàn bộ thư mục `code` sang `backup\code_v1` (bao gồm cả nội dung bên trong)

-Copy-Item -Path "smart-farm\code" -Destination "smart-farm\backup\code_v1" -Recurse
