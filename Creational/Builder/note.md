## Builder Pattern

1. **Mục đích**
- Giúp tạo ra đối phức tạp một cách dễ dàng hơn, dễ quản lý và mở rộng hơn. Việc tạo đối tượng sẽ chia thành các bước nhỏ để dễ dàng kiểm soát
- Giảm sự phụ thuộc vào hàm constructor. Vì đã chia thành nhiều bước nhỏ nên sẽ dể hiểu hơn
- Có tính linh hoạt cao, dễ dàng mở rộng
2. **Nên sử dụng khi nào**
- Cần tạo 1 đối tượng phức tạp và có nhiều tham số và cần thám số có thể tùy chỉnh
- Việc tạo đối tượng cần nhiều bước
- Muốn kiểm soát việc tạo đối tượng 1 cách dễ dàng
- Việc tạo đối tượng có quá nhiều tham số trong constructor và muốn giảm phụ thuộc vào nó
3. **Cấu trúc**
- Builder: thường là abtract class hoặc interface để định nghĩa các phương thức của class
- ConcreteBuilder: Là các lớp triển khai của builder. Mỗi class này sẽ biểu diễn cụ thể đối tượng
- Director: là phần sử dụng builder để tạo ra 1 đối tượng cụ thể.
- Product: là đối tượng phức tạp cuối cùng được xây dựng
4. **Nhược điểm**
- Cấu trúc có thể trở nên phức tạp hơn khi có nhiều lớp Builder.
- Có thể dẫn đến việc tạo ra quá nhiều lớp, đặc biệt là khi chỉ cần một đối tượng đơn giản.

Tham khảo: https://refactoring.guru/design-patterns/builder
