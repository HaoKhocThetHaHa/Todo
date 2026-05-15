# Todo Console App

Ứng dụng quản lý công việc đơn giản được xây dựng bằng C# Console App theo mô hình phân tầng gồm UI, Service và Repository.

## Chức năng

- Hiển thị danh sách công việc
- Thêm công việc mới
- Sửa nội dung công việc
- Xoá công việc
- Đánh dấu hoàn thành công việc
- Lưu dữ liệu vào file `todos.txt`

---

## Công nghệ sử dụng

- C#
- .NET Console Application
- File Handling (`System.IO`)
- LINQ

---

## Cấu trúc project

```text
Todo
│
├── Program.cs
├── Todo.cs
├── TodoRepository.cs
├── TodoService.cs
├── TodoUI.cs
└── todos.txt
```

---

## Mô tả các file

### Program.cs
Điểm bắt đầu của chương trình.

```csharp
new TodoUI().Run();
```

---

### Todo.cs
Chứa model Todo gồm:
- Id
- Title
- IsSuccess

Ngoài ra còn hỗ trợ:
- Chuyển object thành chuỗi để lưu file
- Đọc dữ liệu từ file

---

### TodoRepository.cs
Xử lý:
- Lưu dữ liệu
- Đọc dữ liệu từ file
- CRUD Todo

Dữ liệu được lưu trong file:

```text
todos.txt
```

---

### TodoService.cs
Lớp trung gian xử lý logic giữa UI và Repository.

---

### TodoUI.cs
Hiển thị menu console và tương tác với người dùng.

Menu gồm:

```text
1. Thêm mới công việc
2. Đánh dấu công việc
3. Sửa công việc
4. Xoá công việc
0. Thoát
```

---

## Cách chạy chương trình

### Yêu cầu
- Visual Studio 2022
- .NET SDK

### Chạy project

1. Clone project:

```bash
git clone <repository-url>
```

2. Mở bằng Visual Studio

3. Nhấn:

```text
Ctrl + F5
```

hoặc:

```text
F5
```

---

## Dữ liệu lưu trữ

Dữ liệu Todo được lưu dưới dạng text trong file:

```text
todos.txt
```

Ví dụ:

```text
0:Học C#:False
1:Làm bài tập:True
```

---

## Giao diện chương trình

```text
====DANH SÁCH CÔNG VIỆC====

[ ] 0:Học C#
[x] 1:Làm bài tập

1. Thêm mới công việc
2. Đánh dấu công việc
3. Sửa công việc
4. Xoá công việc
0. Thoát
```

---

## Kiến thức áp dụng

- Lập trình hướng đối tượng (OOP)
- CRUD cơ bản
- Xử lý file trong C#
- Phân tầng ứng dụng
- Sử dụng List và LINQ

---

## Hướng phát triển

- Thêm tìm kiếm công việc
- Thêm deadline
- Kết nối SQL Server
- Xây dựng giao diện WinForms/WPF
- Phát triển thành Web API ASP.NET

---

## Tác giả

- Dương Công Hảo
