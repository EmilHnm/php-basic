# PHP Basic

Thực hiện bởi [Ngô Minh Hoà](https://github.com/EmilRailgun)

## Web Technology

Công nghệ web (Web Technology) đề cập đến các công cụ và kỹ thuật khác nhau được sử dụng trong quá trình giao tiếp giữa các loại thiết bị khác nhau qua internet. Một trình duyệt web được sử dụng để truy cập các trang web. Trình duyệt web có thể được định nghĩa là các chương trình hiển thị văn bản, dữ liệu, hình ảnh, hoạt ảnh và video trên Internet. Các tài nguyên siêu liên kết trên World Wide Web có thể được truy cập bằng các giao diện phần mềm do trình duyệt Web cung cấp.

## HTML5 và CSS

### HTML5

HTML, viết tắt của <strong>HyperText Markup Language</strong>, được sử dụng để thiết kế các trang web bằng ngôn ngữ đánh dấu. HTML là ghép bởi của HyperText (Siêu văn bản) và Markup Language (Ngôn ngữ đánh dấu). HyperText xác định liên kết giữa các trang web. Markup Language được sử dụng để xác định tài liệu văn bản trong thẻ xác định cấu trúc của các trang web. HTML 5 là phiên bản thứ năm và là hiện tại của HTML. Nó đã cải thiện đánh dấu có sẵn cho các tài liệu và đã giới thiệu các giao diện lập trình ứng dụng (API) và Mô hình đối tượng tài liệu (DOM).

### CSS

Cascading Style Sheets, hay còn được gọi là CSS, là một ngôn ngữ được thiết kế đơn giản nhằm mục đích đơn giản hóa quá trình làm cho các trang web có thể hiển thị được. CSS cho phép bạn áp dụng các kiểu (style) cho các trang web. Quan trọng hơn, CSS cho phép bạn thực hiện điều này độc lập với HTML tạo nên mỗi trang web. Nó mô tả giao diện của một trang web: nó quy định màu sắc, phông chữ, khoảng cách, v.v. Nói tóm lại, bạn có thể làm cho trang web của mình trông như thế nào bạn muốn. CSS cho phép các nhà phát triển và nhà thiết kế xác định cách nó hoạt động, bao gồm cả cách các phần tử được định vị trong trình duyệt.

## PHP

PHP là từ viết tắt của PHP: Hypertext Preprocessor. PHP là ngôn ngữ kịch bản phía máy chủ được thiết kế dành riêng cho phát triển web. Nó rất đơn giản để tìm hiểu và sử dụng. Các tệp có phần mở rộng là “.php”.

## PHP Syntax

Tập lệnh PHP có thể được đặt ở bất kỳ đâu trong tài liệu.

Một tập lệnh PHP bắt đầu bằng `<?php` và kết thúc bằng `?>` :

```php
<?php
// Write your PHP code here
?>
```

## PHP Datatype

Trong PHP có 8 kiểu dữ liệu cơ bản:

- String
- Integer
- Float (floating point numbers - also called double)
- Boolean
- Array
- Object
- NULL
- Resource

### String (Chuỗi)

<strong>String</strong> là một chuỗi các ký tự. Một chuỗi có thể là một từ, một câu hoặc một đoạn văn bản. Một chuỗi có thể được xác định bằng cách đặt nó trong dấu nháy đơn hoặc nháy kép:

```php
<?php
$x = "Hello world!";
$y = 'Hello world!';
?>
```

### Integer (Số nguyên)

Kiểu dữ liệu <strong>Integer</strong> là số không phải số thập phân trong khoảng từ -2.147.483.648 đến 2.147.483.647.

```php
<?php
$x = 2022;
$y = -2022;
?>
```

### Float (Số thực)

Kiểu <strong>Float</strong> (số dấu phẩy động) là một số có dấu thập phân hoặc một số ở dạng số mũ.

```php
<?php
$x = 2022.11;
?>
```

### Boolean

<strong>Boolean</strong> đại diện cho hai trạng thái có thể xảy ra: <strong>TRUE</strong> hoặc <strong>FALSE</strong>.

```php
<?php
$x = true;
$y = false;
?>
```

### Array (Mảng)

MỘt mảng lưu trữ nhiều giá trị trong một biến duy nhất.

```php
<?php
$classes = array("Warrior","Archer","Mage");
?>
```

### Object (Đối tượng)

Lớp (class) và đối tượng (object) là hai khái niệm cơ bản của OOP. Một lớp là một mô hình để tạo ra các đối tượng. Một đối tượng là một thực thể của lớp.

```php
<?php
class Classes {
    public $name;
    public $weapon;
  function Classes($name, $weapon) {
    $this->name = $name;
    $this->weapon = $weapon;
  }
}

$warrior = new Classe("Warrior","Sword");
$archer = new Classes("Archer","Bow");
```

### NULL

Giá trị <strong>NULL</strong> là giá trị không có giá trị. Nó là một kiểu dữ liệu đặc biệt, chỉ có một giá trị: <strong>NULL</strong>.

```php
<?php
$x = "Hello world!";
$x = null;
?>
```

### Resource (Tài nguyên)

Một tài nguyên là một biến chứa một tham chiếu đến một tài nguyên bên ngoài - chẳng hạn như một tệp được mở bởi PHP, hoặc một kết nối đến cơ sở dữ liệu.

## PHP Variables, Constants, Arrays

### Variables (Biến)

Một biến là một tên được sử dụng để lưu trữ một giá trị. Biến có thể chứa các giá trị khác nhau, và có thể được thay đổi trong suốt quá trình chạy chương trình.

Một biến được khởi tạo bằng cách sử dụng dấu `$` theo sau bởi tên của biến.

```php
<?php
$txt = "Hello world!";
$x = 2022;
$y = 2022.11;
?>
```

### Constants (Hằng)

Một hằng số là một tên (một biến) cho một giá trị. Một hằng số không thể thay đổi sau khi nó được định nghĩa.

Một hằng số được định nghĩa bằng cách sử dụng hàm `define()`.

```php
<?php
define("constant", "Hello I'm a constant!");
echo constant;
?>
```

### Arrays (Mảng)

Một mảng lưu trữ nhiều giá trị trong một biến duy nhất.

Có 3 loại mảng trong PHP:

- Indexed arrays - Mảng có chỉ số
- Associative arrays - Mảng có khóa
- Multidimensional arrays - Mảng đa chiều

## PHP Operators (Toán tử)

Toán tử được sử dụng để thực hiện các phép toán trên các biến và giá trị. Toán tử được chia thành các nhóm sau:

- Toán tử số học
- Toán tử gán
- Toán tử so sánh
- Toán tử tăng/giảm
- Toán tử logic
- Toán tử chuỗi
- Toán tử mảng
- Toán tử gán có điều kiện

## Control Structures (Cấu trúc điều khiển)

Cấu trúc điều khiển là một cách để thực hiện các hành động khác nhau dựa trên các điều kiện khác nhau.

### if...else (Nếu...thì)

Rất được sử dụng trong các trường hợp cần kiểm tra điều kiện để chạy đoạn mã cần thiết trong trường hợp nhất định.

Cú pháp:

```php
<?php
if (condition) {
  // code to be executed if condition is true
} else {
  // code to be executed if condition is false
}
?>
```

### switch...case (Chuyển...trường hợp)

Câu lệnh `switch` được sử dụng để thực hiện các hành động khác nhau dựa trên các điều kiện khác nhau.

Cú pháp:

```php
<?php
switch (n) {
  case label1:
    code to be executed if n=label1;
    break;
  case label2:
    code to be executed if n=label2;
    break;
  case label3:
    code to be executed if n=label3;
    break;
  ...
  default:
    code to be executed if n is different from all labels;
}
?>
```

## Loops (Vòng lặp)

Vòng lặp được sử dụng để thực hiện một khối mã (code block) nhiều lần trong khi điều kiện được chỉ định là đúng.

### while (Trong khi)

Cú pháp:

```php
<?php
while (condition is true) {
  code to be executed;
}
?>
```

### do...while (Làm...trong khi)

Cú pháp:

```php
<?php
do {
  code to be executed;
} while (condition is true);
?>
```

### for (Với)

Cú pháp:

```php
<?php
for (init counter; test counter; increment counter) {
  code to be executed;
}
?>
```

### foreach (Với mỗi)

Cú pháp:

```php
<?php
foreach ($array as $value) {
  code to be executed;
}
?>
```

## String Functions (Hàm chuỗi)

Hàm chuỗi được sử dụng để thao tác với chuỗi. Một số hàm chuỗi thường được sử dụng:

- `strlen()` - Độ dài chuỗi
- `str_word_count()` - Đếm số từ trong chuỗi
- `strrev()` - Đảo ngược chuỗi
- `strpos()` - Tìm vị trí của một chuỗi con trong chuỗi
- `str_replace()` - Thay thế chuỗi con trong chuỗi
- `substr()` - Trích xuất một phần của chuỗi
- `strtolower()` - Chuyển chuỗi thành chữ thường
- `strtoupper()` - Chuyển chuỗi thành chữ hoa
- `ucfirst()` - Chuyển chữ cái đầu tiên của chuỗi thành chữ hoa
- `ucwords()` - Chuyển chữ cái đầu tiên của mỗi từ trong chuỗi thành chữ hoa
- `trim()` - Loại bỏ khoảng trắng ở đầu và cuối chuỗi
- `ltrim()` - Loại bỏ khoảng trắng ở đầu chuỗi
- `rtrim()` - Loại bỏ khoảng trắng ở cuối chuỗi
- ...

## Array Functions (Hàm mảng)

Hàm mảng được sử dụng để thao tác với mảng. Một số hàm mảng thường được sử dụng:

- `count()` - Đếm số phần tử trong mảng
- `array_sum()` - Tính tổng các phần tử trong mảng
- `array_product()` - Tính tích các phần tử trong mảng
- `array_reverse()` - Đảo ngược mảng
- `in_array()` - Kiểm tra một phần tử có tồn tại trong mảng hay không
- `array_rand()` - Trả về một phần tử ngẫu nhiên trong mảng
- `array_unique()` - Loại bỏ các phần tử trùng lặp trong mảng
- `array_merge()` - Gộp hai mảng
- `sort()` - Sắp xếp mảng theo thứ tự tăng dần
- `rsort()` - Sắp xếp mảng theo thứ tự giảm dần
- ...

## File Handling (Xử lý tập tin)

Xử lý tập tin được sử dụng để thao tác với tập tin. Một số hàm xử lý tập tin thường được sử dụng:

- `fopen()` - Mở tập tin
- `fclose()` - Đóng tập tin
- `fread()` - Đọc tập tin
- `fwrite()` - Ghi tập tin
- `feof()` - Kiểm tra xem con trỏ đã đến cuối tập tin hay chưa
- `fgetc()` - Đọc ký tự tại vị trí con trỏ đang trỏ tới
- `fgets()` - Đọc một dòng tại vị trí con trỏ đang trỏ tới
- `fgetcsv()` - Đọc một dòng tại vị trí con trỏ đang trỏ tới và chuyển thành mảng
- `fputcsv()` - Ghi một dòng vào tập tin và chuyển thành mảng
- `file()` - Đọc tập tin và chuyển thành mảng
- . . .

## nginx, apache, web-stack, php-fpm

### Nginx

Nginx là một web server, được phát triển bởi Igor Sysoev. Nginx được thiết kế để hỗ trợ tải các dữ liệu lớn, cung cấp các tính năng như load balancing, caching, reverse proxying, và HTTP accelerator. Nginx cũng có thể được sử dụng như một proxy mail (IMAP/POP3) và HTTP.

### Apache

<strong>Apache</strong> là một web server, được phát triển bởi Apache Software Foundation với tên chính thức là <strong>Apache HTTP Server</strong>. Apache được sử dụng rộng rãi trên các hệ điều hành Unix, Linux, Windows, và Mac OS X.

### Web-stack

Web-stack là một tập hợp các phần mềm cần thiết để xây dựng một ứng dụng web. Web-stack bao gồm các phần mềm sau:

- Web server: Nginx, Apache, IIS
- Database: MySQL, PostgreSQL, MongoDB
- Language: PHP, Python, Ruby, NodeJS
- Framework: Laravel, Django, Ruby on Rails, ExpressJS
- ...

### PHP-FPM

PHP-FPM là một FastCGI Process Manager, được sử dụng để xử lý các request PHP. PHP-FPM được sử dụng để tăng hiệu năng của PHP, đồng thời giảm thiểu tải cho web server.
