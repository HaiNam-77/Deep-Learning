# 🧠 Deep Learning: Foundations & PyTorch Implementation

Repository này lưu trữ tài liệu lý thuyết nền tảng và mã nguồn thực nghiệm các mô hình Học sâu (Deep Learning) từ cơ bản đến nâng cao sử dụng framework **PyTorch**.

---

## 📂 Cấu trúc Repository

- **[Code/](./Code):** Chứa mã nguồn cài đặt mạng nơ-ron và thuật toán tối ưu (PyTorch).
- **[Lý Thuyết/](./L%C3%BD%20Thuy%E1%BA%BFt):** Chứa ghi chép chi tiết về cơ sở toán học, kiến trúc mạng và lan truyền ngược.

---

## 📌 Nội dung chi tiết các thư mục

### 1. [Lý Thuyết - Cơ chế & Nền tảng](./L%C3%BD%20Thuy%E1%BA%BFt)
Nghiên cứu nguyên lý toán học đằng sau các thành phần của mạng nơ-ron:
- **Kiến trúc Mạng nơ-ron:** Bản chất perceptron, mô hình mạng truyền thẳng đa tầng (Multi-Layer Perceptron - MLP).
- **Cơ chế Lan truyền:** Quá trình truyền tiến (Forward Pass), tính toán hàm mất mát (Loss functions như MSE, Cross-Entropy) và lan truyền ngược (Backpropagation) để cập nhật gradient.
- **Hàm kích hoạt:** Khảo sát các hàm phi tuyến tính như ReLU, Sigmoid, Tanh và Softmax.
- **Thuật toán Tối ưu hóa:** Cơ sở lý thuyết của Gradient Descent, cơ chế bổ sung quán tính (Momentum) và thích ứng tốc độ học (Adaptive Learning Rate trong Adam, RMSprop).

### 2. [Code - Triển khai Thực nghiệm với PyTorch](./Code)
Triển khai mã nguồn thực tế:
- **MLP Implementation (`MLP_code.ipynb`):** Tự xây dựng pipeline huấn luyện mạng nơ-ron hoàn chỉnh với `torch.nn.Module`, thiết lập vòng lặp huấn luyện (training loop), theo dõi hàm mất mát và đánh giá độ chính xác (Accuracy).
- **Optimizers Comparison (`Optimizer_code.ipynb`):** Cài đặt, đo lường và vẽ biểu đồ so sánh trực tiếp tốc độ hội tụ cũng như độ ổn định giữa các bộ tối ưu hóa (SGD, SGD with Momentum, RMSprop, Adam) trên cùng một bài toán.

---

## 🛠️ Công nghệ & Công cụ sử dụng

- **Ngôn ngữ:** Python 3
- **Thư viện Deep Learning:** PyTorch (`torch`, `torch.nn`, `torch.optim`)
- **Xử lý & Trực quan hóa dữ liệu:** NumPy, Matplotlib
- **Môi trường thực thi:** Jupyter Notebook / Google Colab
