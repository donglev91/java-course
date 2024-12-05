# Làm quen: Why && how

## History
- **Java là gì?** 
  - Java là một ngôn ngữ lập trình hướng đối tượng, được thiết kế để có thể chạy trên nhiều nền tảng khác nhau.
- **Viết ra bởi ai?**
  - Được phát triển bởi Sun Microsystems (hiện nay là một phần của Oracle Corporation), đặc biệt là bởi James Gosling và đội ngũ của ông vào những năm 1990.
- **Tại sao dùng Java trong thời điểm ấy? Java giải quyết bài toán gì?**
  - Java được thiết kế để giải quyết vấn đề về tính tương thích và khả năng di động của phần mềm. Bằng cách sử dụng mô hình "viết một lần, chạy mọi nơi" (Write Once, Run Anywhere), Java giúp các nhà phát triển có thể viết mã một lần và chạy trên bất kỳ nền tảng nào hỗ trợ Java mà không cần sửa đổi nhiều.

## Các thành phần cơ bản của Java
- **JDK (Java Development Kit):**
  - Bộ công cụ phát triển bao gồm trình biên dịch, thư viện chuẩn, và các công cụ phát triển cần thiết để viết, biên dịch và chạy mã Java.
- **JRE (Java Runtime Environment):**
  - Môi trường chạy cho các chương trình Java, bao gồm Java Virtual Machine (JVM) và các thư viện lớp cần thiết để chạy các ứng dụng được phát triển bằng Java.

## Viết test Java Hello world
- **Bước 1:** Tạo một tệp tin Java mới và đặt tên là `HelloWorld.java`.
- **Bước 2:** Viết mã nguồn Java cơ bản:
  ```java
  public class HelloWorld {
      public static void main(String[] args) {
          System.out.println("Hello, World!");
      }
  }

# Hướng dẫn tạo tài khoản GitHub và đẩy code lên GitHub

## Bước 1: Tạo tài khoản GitHub
1. Truy cập trang web [github.com](https://github.com) và nhấn vào nút **Sign up**.
2. Nhập thông tin cá nhân của bạn bao gồm địa chỉ email, mật khẩu, và tên người dùng. 
3. Xác nhận email của bạn thông qua email mà GitHub gửi đến.
4. Hoàn thành các bước hướng dẫn còn lại để thiết lập tài khoản của bạn.

## Bước 2: Thiết lập Git trên máy tính
1. Tải và cài đặt Git từ trang web [git-scm.com](https://git-scm.com).
2. Sau khi cài đặt, mở terminal (hoặc Command Prompt trên Windows).
3. Cấu hình thông tin người dùng của bạn:
   ```bash
   git config --global user.name "Tên của bạn"
   git config --global user.email "email@example.com"

git init
git add .
git commit -m "First commit"
git remote add origin <repository-url>
git push -u origin master


# Cú pháp cơ bản

## Biến, hằng, các kiểu dữ liệu
- **Biến:** Dùng để lưu trữ giá trị, có thể thay đổi trong quá trình thực thi chương trình.
  - Cú pháp khai báo biến: `int a = 10;`
- **Hằng:** Giá trị cố định không thay đổi.
  - Cú pháp khai báo hằng: `final int MAX = 100;`
- **Các kiểu dữ liệu:**
  - **Số nguyên:** `int`, `byte`, `short`, `long`
  - **Số thực:** `float`, `double`
  - **Ký tự:** `char`
  - **Boolean:** `boolean` (true/false)
  - **Chuỗi:** `String`
  - **Ví dụ:**
    ```java
    int age = 25;
    float height = 5.8f;
    char gender = 'M';
    boolean isStudent = true;
    String name = "John";
    ```

## Các toán tử
- **Logic:** 
  - AND: `&&`
  - OR: `||`
  - NOT: `!`
- **Số học:**
  - Cộng: `+`
  - Trừ: `-`
  - Nhân: `*`
  - Chia: `/`
  - Chia lấy dư: `%`
- **Một ngôi:**
  - Tăng: `++`
  - Giảm: `--`
  - Dấu âm: `-`
  - Dấu dương: `+`
- **Ví dụ:**
  ```java
  int x = 10;
  int y = 20;
  int sum = x + y; // Kết quả: 30
  int difference = x - y; // Kết quả: -10
  int product = x * y; // Kết quả: 200
  int quotient = x / y; // Kết quả: 0
  int remainder = x % y; // Kết quả: 10
  boolean result = (x < y) && (x > 5); // Kết quả: true
  x++; // Kết quả: 11
  y--; // Kết quả: 19
# Kiểu dữ liệu nâng cao

## Mảng
- **Mảng (Array):**
  - Mảng là cấu trúc dữ liệu lưu trữ nhiều giá trị có cùng kiểu dữ liệu.
  - Các phần tử trong mảng được lưu trữ liên tiếp nhau trong bộ nhớ.
  - Cú pháp khai báo mảng:
    ```java
    int[] arr = new int[10]; // Khai báo mảng kiểu int với 10 phần tử
    int[] numbers = {1, 2, 3, 4, 5}; // Khởi tạo mảng với các giá trị ban đầu
    ```
  - Truy cập phần tử trong mảng:
    ```java
    int firstElement = numbers[0]; // Truy cập phần tử đầu tiên
    numbers[2] = 10; // Gán giá trị cho phần tử thứ 3
    ```

## Đối tượng
- **Đối tượng (Object):**
  - Đối tượng là thực thể có trạng thái và hành vi.
  - Được tạo từ lớp (class), chứa các thuộc tính (properties) và phương thức (methods).
  - Ví dụ về lớp và đối tượng:
    ```java
    // Định nghĩa lớp
    public class Person {
        String name;
        int age;

        // Constructor
        public Person(String name, int age) {
            this.name = name;
            this.age = age;
        }

        // Phương thức hiển thị thông tin
        public void display() {
            System.out.println("Name: " + name);
            System.out.println("Age: " + age);
        }
    }

    // Tạo đối tượng
    Person person = new Person("Alice", 30);
    person.display(); // Gọi phương thức của đối tượng
    ```

## Map và HashMap
- **Map:**
  - Map là cấu trúc dữ liệu lưu trữ các cặp key-value.
  - Cho phép truy cập nhanh chóng đến giá trị thông qua key.
- **HashMap:**
  - Là một triển khai của Map, lưu trữ các cặp key-value.
  - Các key trong HashMap là duy nhất và không theo thứ tự.
  - Cú pháp sử dụng HashMap:
    ```java
    import java.util.HashMap;

    HashMap<String, Integer> map = new HashMap<>();
    map.put("apple", 10);
    map.put("banana", 20);

    int value = map.get("apple"); // Truy cập giá trị thông qua key
    System.out.println("Value of apple: " + value);
    ```

## ArrayList và List
- **ArrayList:**
  - ArrayList là một danh sách động, cho phép lưu trữ các phần tử và tự động mở rộng kích thước khi cần.
  - Cú pháp sử dụng ArrayList:
    ```java
    import java.util.ArrayList;

    ArrayList<String> list = new ArrayList<>();
    list.add("Java");
    list.add("Python");
    list.add("C++");

    String language = list.get(1); // Truy cập phần tử thứ 2
    System.out.println("Language at index 1: " + language);
    ```
- **List:**
  - List là một giao diện trong Java, đại diện cho một danh sách các phần tử.
  - ArrayList là một triển khai của List.
  - Cú pháp sử dụng List:
    ```java
    import java.util.List;
    import java.util.ArrayList;

    List<String> languages = new ArrayList<>();
    languages.add("Java");
    languages.add("Python");
    languages.add("C++");

    for (String lang : languages) {
        System.out.println(lang);
    }
    ```
# Try, catch, exception handling

## Xử lý ngoại lệ trong Java
- **Ngoại lệ (Exception):**
  - Là các sự cố phát sinh trong quá trình thực thi chương trình, gây ra việc dừng hoạt động của chương trình nếu không được xử lý.
  - Ví dụ: Chia một số cho 0, truy cập một phần tử không tồn tại trong mảng.

- **Các loại ngoại lệ thông dụng:**
  - ArithmeticException: Ngoại lệ số học (vd: chia cho 0)
  - NullPointerException: Ngoại lệ con trỏ null (vd: truy cập phương thức của một đối tượng null)
  - ArrayIndexOutOfBoundsException: Ngoại lệ truy cập chỉ mục ngoài giới hạn của mảng
  - FileNotFoundException: Ngoại lệ tệp tin không tìm thấy
  - IOException: Ngoại lệ vào/ra

- **Lợi ích của việc xử lý ngoại lệ:**
  - Giúp chương trình hoạt động ổn định và không bị dừng đột ngột khi gặp lỗi.
  - Tăng cường khả năng bảo trì và đọc hiểu mã nguồn.
  - Giúp phát hiện và khắc phục lỗi một cách dễ dàng và rõ ràng hơn.

## Try, catch, finally
- **Try:** Khối mã mà bạn muốn thử thực hiện và có thể phát sinh ngoại lệ.
- **Catch:** Khối mã dùng để xử lý ngoại lệ nếu nó phát sinh trong khối try.
- **Finally:** Khối mã sẽ luôn được thực thi dù có hay không có ngoại lệ phát sinh.


## Cú pháp xử lý ngoại lệ
```java
try {
    // Mã có thể gây ra ngoại lệ
} catch (ExceptionType e) {
    // Mã xử lý ngoại lệ
} finally {
    // Mã luôn được thực thi
}

public class ExceptionExample {
    public static void main(String[] args) {
        try {
            int result = 10 / 0; // Gây ra ngoại lệ ArithmeticException
        } catch (ArithmeticException e) {
            System.out.println("Cannot divide by zero."); // Xử lý ngoại lệ
        } finally {
            System.out.println("This block is always executed."); // Khối finally
        }
    }
}
```

# Date time

## Sử dụng lớp `Date` trong Java
- **Lớp `Date`:** Lớp này đại diện cho một điểm thời gian cụ thể, chính xác đến mili giây kể từ mốc thời gian (epoch) là 00:00:00 ngày 1 tháng 1 năm 1970.
- **Khởi tạo đối tượng `Date`:**
  ```java
  import java.util.Date;

  public class DateExample {
      public static void main(String[] args) {
          Date currentDate = new Date();
          System.out.println("Current date: " + currentDate);
      }
  }


