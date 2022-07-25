1. Nhận diện làn đường
- chạy terminal: python main.py -i "video đầu vào" -o "vid đầu ra"
ví dụ: python main.py -i "./1.mp4" -o "./res/res1.mp4"
- trong file gui.py, sửa lại dòng 15, 16 là đường dẫn vid đầu vào và đầu ra ở trên.
- chạy  python gui.py để hiển thị kết quả

2. Nhận diện phương tiện giao thông
- chạy terminal: 
    pip install -qr requirements.txt
    python : import torch
             import utils
             display = utils.notebook_init()
- Tải ảnh cho vào thư mục ./nhan dien phuong tien giao thong/yolov5/data/images    
- chạy terminal: python detect.py --weights ./runs/train/exp3/weights/best.pt --img 640 --conf 0.25 --source data/images/(tên ảnh, vd: img.jpg, a.mp4, ...)
- Kết quả sẽ được lưu vào các thư mục runs/detect/exp
         