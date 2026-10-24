# 🧠 Deep Learning - Implementation & Optimization

Thư mục này chứa mã nguồn cài đặt các kiến trúc mạng nơ-ron nền tảng và thử nghiệm các thuật toán tối ưu hóa (Optimizers) trong Deep Learning sử dụng **PyTorch**.

---

## 📌 Nội dung thực nghiệm (Notebooks)

### 1. [MLP_code.ipynb](./MLP_code.ipynb)
- **Kiến trúc:** Mạng nơ-ron truyền thẳng đa tầng (Multi-Layer Perceptron - MLP).
- **Mục tiêu:** Cài đặt từ nền tảng quy trình huấn luyện mạng nơ-ron cho bài toán phân loại dữ liệu (Classification).
- **Kỹ thuật chính:**
  - Thiết kế các tầng kết nối đầy đủ (Fully Connected / Linear Layers) với `torch.nn.Linear`.
  - Thực nghiệm các hàm kích hoạt phi tuyến tính (Activation Functions): ReLU, Sigmoid, Tanh.
  - Xử lý lan truyền tiến (Forward Pass), tính toán hàm mất mát (Loss Function như Cross-Entropy Loss) và lan truyền ngược (Backpropagation) để cập nhật trọng số.
  - Đánh giá độ chính xác (Accuracy) và theo dõi hiện tượng Overfitting qua từng epoch.

---

### 2. [Optimizer_code.ipynb](./Optimizer_code.ipynb)
- **Chủ đề:** Các thuật toán tối ưu hóa (Optimization Algorithms) trong quá trình huấn luyện mô hình.
- **Mục tiêu:** So sánh tốc độ hội tụ, độ ổn định và hiệu năng của các thuật toán Gradient Descent khác nhau.
- **Kỹ thuật chính:**
  - Cài đặt và thực nghiệm các thuật toán tối ưu:
    - **SGD (Stochastic Gradient Descent):** Cập nhật trọng số theo từng mẫu/batch nhỏ.
    - **SGD with Momentum:** Bổ sung quán tính giúp vượt qua các điểm cực tiểu địa phương (local minima) và vùng yên ngựa (saddle points).
    - **RMSprop / AdaGrad:** Tự động điều chỉnh tốc độ học (adaptive learning rate) theo từng trọng số.
    - **Adam (Adaptive Moment Estimation):** Kết hợp ưu điểm của Momentum và RMSprop, theo dõi gradient bậc 1 và bậc 2.
  - Vẽ đồ thị so sánh đường cong suy giảm hàm mất mát (Loss Curve) giữa các Optimizer.

---

## 🛠️ Công nghệ & Thư viện sử dụng

- **Ngôn ngữ:** Python 3
- **Thư viện Deep Learning:** PyTorch (`torch`, `torch.nn`, `torch.optim`)
- **Phân tích & Hiển thị dữ liệu:** NumPy, Matplotlib, Seaborn
- **Môi trường thực thi:** Jupyter Notebook / Google Colab

---

> 💡 *Phần lý thuyết chi tiết, công thức toán học và giải thích cơ chế của MLP cùng Optimizers được lưu trữ tại thư mục [../Lý Thuyết](../Lý%20Thuyết).*
