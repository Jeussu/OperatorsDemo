# Operators
51. Operators

51. Người điều hành

Toán tử trong C# là các ký hiệu hoặc từ khóa thực hiện các thao tác cụ thể trên toán hạng (biến, hằng hoặc ký tự) và tạo ra kết quả. Có nhiều loại toán tử khác nhau trong C#, được phân loại thành các nhóm sau:

1. Toán tử số học:
    - Phép cộng (+): Cộng hai toán hạng.
    - Subtraction (-): Trừ toán hạng bên phải cho toán hạng bên trái.
    - Phép nhân (*): Nhân hai toán hạng.
    - Phép chia (/): Chia toán hạng bên trái cho toán hạng bên phải.
    - Modulus (%): Trả về phần dư của phép chia toán hạng bên trái cho toán hạng bên phải.
    - Increment (++) và Decrement (--): Dùng để tăng hoặc giảm giá trị của toán hạng đi 1 đơn vị.

2. Các toán tử quan hệ:
    - Equal to (==): Kiểm tra xem hai toán hạng có bằng nhau không.
    - Not equal to (!=): Kiểm tra xem hai toán hạng có bằng nhau không.
    - Lớn hơn (>): Kiểm tra xem toán hạng bên trái có lớn hơn toán hạng bên phải hay không.
    - Nhỏ hơn (<): Kiểm tra xem toán hạng bên trái có nhỏ hơn toán hạng bên phải hay không.
    - Lớn hơn hoặc bằng (>=): Kiểm tra xem toán hạng bên trái có lớn hơn hoặc bằng toán hạng bên phải hay không.
    - Nhỏ hơn hoặc bằng (<=): Kiểm tra xem toán hạng bên trái có nhỏ hơn hoặc bằng toán hạng bên phải hay không.

3. Toán tử logic:
    - Logic AND (&&): Trả về true nếu cả hai toán hạng đều true.
    - Logic OR (||): Trả về true nếu ít nhất một trong các toán hạng là true.
    - Logical NOT (!): Đảo ngược trạng thái logic của toán hạng của nó.

4. Toán tử chuyển nhượng:
    - Phép gán (=): Gán giá trị của toán hạng bên phải cho toán hạng bên trái.
    - Toán tử gán tổ hợp (ví dụ: +=, -=, *=, /=): Thực hiện phép toán và gán kết quả cho toán hạng bên trái.

5. Toán tử Bitwise:
    - Bitwise AND (&): Thực hiện thao tác AND theo bit trên biểu diễn nhị phân của hai toán hạng.
    - Bitwise OR (|): Thực hiện phép toán OR theo bit trên biểu diễn nhị phân của hai toán hạng.
    - Bitwise XOR (^): Thực hiện thao tác OR loại trừ bitwise trên biểu diễn nhị phân của hai toán hạng.
    - Bitwise NOT (~): Đảo ngược các bit của toán hạng của nó.
    - Dịch trái (<<): Dịch các bit của toán hạng bên trái sang trái theo số vị trí do toán hạng bên phải chỉ định.
    - Dịch phải (>>): Dịch các bit của toán hạng bên trái sang phải theo số vị trí do toán hạng bên phải chỉ định.

6. Toán tử bậc ba (? :):
    - Toán tử if-else rút gọn trả về một trong hai giá trị dựa trên một điều kiện.

7. Các toán tử khác:
    - Toán tử truy cập thành viên (.): Truy cập các thành viên (trường, thuộc tính, phương thức) của một lớp hoặc cấu trúc.
    - Toán tử truy cập thành viên có điều kiện (?.): Truy cập các thành viên của một đối tượng nếu đối tượng không phải là null.
    - Toán tử chỉ mục ([]): Truy cập các phần tử của mảng hoặc tập hợp theo chỉ mục.
    - Toán tử truyền kiểu (e.g., (int), (double), (string)): Chuyển đổi kiểu dữ liệu này sang kiểu dữ liệu khác.

Ví dụ về việc sử dụng các toán tử số học:
```csharp
int a = 10, b = 5;
int sum = a + b; // 15
int difference = a - b; // 5
int product = a * b; // 50
int quotient = a / b; // 2
int remainder = a % b; // 0
```
Ví dụ sử dụng toán tử quan hệ:
```csharp
bool isEqual = a == b; // false
bool isNotEqual = a != b; // true
bool isGreater = a > b; // true
bool isLess = a < b; // false
bool isGreaterOrEqual = a >= b; // true
bool isLessOrEqual = a <= b; // false
```

Các toán tử này là nền tảng để thực hiện tính toán, đưa ra quyết định và kiểm soát luồng chương trình trong các ứng dụng C#.

My Code:
namespace OperatorsC
{
    class Program
    {
        static void Main(string[] args)
        {
            int num1 = 5;
            int num2 = 3;
            int num3;

            // unary operators
            num3 = -num1;
            Console.WriteLine("num3 is {0}", num3);

            bool isSunny = true;
            Console.WriteLine("is it sunny? {0}", !isSunny);

            // increment operators 
            int num = 0;
            num++;
            Console.WriteLine("num is {0}", num);
            Console.WriteLine("num is {0}", num++);
            // pre increment
            Console.WriteLine("num is {0}", ++num);

            // decrement operator
            num--;
            Console.WriteLine("num is {0}", num);
            Console.WriteLine("num is {0}", num--);
            // pre decrement
            Console.WriteLine("num is {0}", --num);

            int result;
            result = num1 + num2;
            Console.WriteLine("result of num1 + num2 is {0}", result);
            result = num1 - num2;
            Console.WriteLine("result of num1 - num2 is {0}", result);
            result = num1 / num2;
            Console.WriteLine("result of num1 / num2 is {0}", result);
            result = num1 * num2;
            Console.WriteLine("result of num1 * num2 is {0}", result);
            result = num1 % num2;
            Console.WriteLine("result of num1 % num2 is {0}", result);

            // relational and type operators
            bool isLower;
            isLower = num1 < num2;
            Console.WriteLine("result of num1 < num2 is {0}", isLower);
            isLower = num1 > num2;
            Console.WriteLine("result of num1 > num2 is {0}", isLower);

            // equality operator
            bool isEqual;
            isEqual = num1 == num2;
            Console.WriteLine("result of num1 == num2 is {0}", isEqual);

            isEqual = (num1 != num2);
            Console.WriteLine("result of num1 != num2 is {0}", isEqual);

            // conditional operators
            bool isLowerAndSunny;
            // condition1 AND condition2
            isLowerAndSunny = isLower && isSunny;
            Console.WriteLine("result of isLower && isSunny is {0}", isLowerAndSunny);

            // condition1 OR condition2
            isLowerAndSunny = isLower || isSunny;
            Console.WriteLine("result of isLower || isSunny is {0}", isLowerAndSunny);

            Console.ReadKey();
        }
    }
}
