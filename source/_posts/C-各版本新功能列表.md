---
title: 'C# 各版本新功能列表'
date: 2020-02-21 11:36:28
tags: .NET
id: new-features-in-csharp
category: 技术汇总
---

>参考资料：[C#发展历史 - C#指南 | Microsoft Docs](https://docs.microsoft.com/zh-cn/dotnet/csharp/whats-new/csharp-version-history
)

# C#各版本新功能列表

- [C#各版本新功能列表](#c%e5%90%84%e7%89%88%e6%9c%ac%e6%96%b0%e5%8a%9f%e8%83%bd%e5%88%97%e8%a1%a8)
  - [C# 2.0版 - 2005](#c-20%e7%89%88---2005)
    - [泛型](#%e6%b3%9b%e5%9e%8b)
    - [分部类型](#%e5%88%86%e9%83%a8%e7%b1%bb%e5%9e%8b)
    - [匿名方法](#%e5%8c%bf%e5%90%8d%e6%96%b9%e6%b3%95)
    - [可以为null的值类型](#%e5%8f%af%e4%bb%a5%e4%b8%banull%e7%9a%84%e5%80%bc%e7%b1%bb%e5%9e%8b)
    - [迭代器](#%e8%bf%ad%e4%bb%a3%e5%99%a8)
    - [协变和逆变](#%e5%8d%8f%e5%8f%98%e5%92%8c%e9%80%86%e5%8f%98)
  - [C# 3.0版 - 2007](#c-30%e7%89%88---2007)
    - [自动实现的属性](#%e8%87%aa%e5%8a%a8%e5%ae%9e%e7%8e%b0%e7%9a%84%e5%b1%9e%e6%80%a7)
    - [匿名类型](#%e5%8c%bf%e5%90%8d%e7%b1%bb%e5%9e%8b)
    - [查询表达式（LINQ）](#%e6%9f%a5%e8%af%a2%e8%a1%a8%e8%be%be%e5%bc%8flinq)
    - [Lambda表达式](#lambda%e8%a1%a8%e8%be%be%e5%bc%8f)
    - [表达式树](#%e8%a1%a8%e8%be%be%e5%bc%8f%e6%a0%91)
    - [扩展方法](#%e6%89%a9%e5%b1%95%e6%96%b9%e6%b3%95)
    - [var](#var)
    - [分部方法](#%e5%88%86%e9%83%a8%e6%96%b9%e6%b3%95)
    - [对象和集合初始值设定项](#%e5%af%b9%e8%b1%a1%e5%92%8c%e9%9b%86%e5%90%88%e5%88%9d%e5%a7%8b%e5%80%bc%e8%ae%be%e5%ae%9a%e9%a1%b9)
  - [C# 4.0版 - 2010](#c-40%e7%89%88---2010)
    - [动态绑定](#%e5%8a%a8%e6%80%81%e7%bb%91%e5%ae%9a)
    - [命名参数/可选参数](#%e5%91%bd%e5%90%8d%e5%8f%82%e6%95%b0%e5%8f%af%e9%80%89%e5%8f%82%e6%95%b0)
    - [泛型中的协变和逆变](#%e6%b3%9b%e5%9e%8b%e4%b8%ad%e7%9a%84%e5%8d%8f%e5%8f%98%e5%92%8c%e9%80%86%e5%8f%98)
    - [类型等效性和嵌入的互操作类型](#%e7%b1%bb%e5%9e%8b%e7%ad%89%e6%95%88%e6%80%a7%e5%92%8c%e5%b5%8c%e5%85%a5%e7%9a%84%e4%ba%92%e6%93%8d%e4%bd%9c%e7%b1%bb%e5%9e%8b)
  - [C# 5.0版 - 2012](#c-50%e7%89%88---2012)
    - [异步编程](#%e5%bc%82%e6%ad%a5%e7%bc%96%e7%a8%8b)
    - [调用方信息](#%e8%b0%83%e7%94%a8%e6%96%b9%e4%bf%a1%e6%81%af)
  - [C# 6.0版 - 2015](#c-60%e7%89%88---2015)
    - [静态导入](#%e9%9d%99%e6%80%81%e5%af%bc%e5%85%a5)
    - [异常筛选器](#%e5%bc%82%e5%b8%b8%e7%ad%9b%e9%80%89%e5%99%a8)
    - [自动初始化表达式](#%e8%87%aa%e5%8a%a8%e5%88%9d%e5%a7%8b%e5%8c%96%e8%a1%a8%e8%be%be%e5%bc%8f)
    - [Expression-bodied 函数成员](#expression-bodied-%e5%87%bd%e6%95%b0%e6%88%90%e5%91%98)
    - [Null传播器](#null%e4%bc%a0%e6%92%ad%e5%99%a8)
    - [字符串内插](#%e5%ad%97%e7%ac%a6%e4%b8%b2%e5%86%85%e6%8f%92)
    - [`nameof`表达式](#nameof%e8%a1%a8%e8%be%be%e5%bc%8f)
    - [索引初始值设定项](#%e7%b4%a2%e5%bc%95%e5%88%9d%e5%a7%8b%e5%80%bc%e8%ae%be%e5%ae%9a%e9%a1%b9)
  - [C# 7.0版 - 2017](#c-70%e7%89%88---2017)
    - [out变量](#out%e5%8f%98%e9%87%8f)
    - [元组和析构函数](#%e5%85%83%e7%bb%84%e5%92%8c%e6%9e%90%e6%9e%84%e5%87%bd%e6%95%b0)
    - [模式匹配](#%e6%a8%a1%e5%bc%8f%e5%8c%b9%e9%85%8d)
    - [本地函数](#%e6%9c%ac%e5%9c%b0%e5%87%bd%e6%95%b0)
    - [更多的expression-bodied成员](#%e6%9b%b4%e5%a4%9a%e7%9a%84expression-bodied%e6%88%90%e5%91%98)
    - [Ref 局部变量和返回结果](#ref-%e5%b1%80%e9%83%a8%e5%8f%98%e9%87%8f%e5%92%8c%e8%bf%94%e5%9b%9e%e7%bb%93%e6%9e%9c)
    - [弃元](#%e5%bc%83%e5%85%83)
    - [二进制文本和数字分隔符](#%e4%ba%8c%e8%bf%9b%e5%88%b6%e6%96%87%e6%9c%ac%e5%92%8c%e6%95%b0%e5%ad%97%e5%88%86%e9%9a%94%e7%ac%a6)
    - [引发表达式](#%e5%bc%95%e5%8f%91%e8%a1%a8%e8%be%be%e5%bc%8f)
  - [C# 8.0版 - 2019](#c-80%e7%89%88---2019)
    - [Readonly 成员](#readonly-%e6%88%90%e5%91%98)
    - [默认接口方法](#%e9%bb%98%e8%ae%a4%e6%8e%a5%e5%8f%a3%e6%96%b9%e6%b3%95)
    - [在更多位置中使用更多模式](#%e5%9c%a8%e6%9b%b4%e5%a4%9a%e4%bd%8d%e7%bd%ae%e4%b8%ad%e4%bd%bf%e7%94%a8%e6%9b%b4%e5%a4%9a%e6%a8%a1%e5%bc%8f)
      - [switch表达式](#switch%e8%a1%a8%e8%be%be%e5%bc%8f)
      - [属性模式](#%e5%b1%9e%e6%80%a7%e6%a8%a1%e5%bc%8f)
      - [元组模式](#%e5%85%83%e7%bb%84%e6%a8%a1%e5%bc%8f)
      - [位置模式](#%e4%bd%8d%e7%bd%ae%e6%a8%a1%e5%bc%8f)
    - [using声明](#using%e5%a3%b0%e6%98%8e)
    - [静态本地函数](#%e9%9d%99%e6%80%81%e6%9c%ac%e5%9c%b0%e5%87%bd%e6%95%b0)
    - [异步流](#%e5%bc%82%e6%ad%a5%e6%b5%81)
    - [索引和范围](#%e7%b4%a2%e5%bc%95%e5%92%8c%e8%8c%83%e5%9b%b4)
    - [Null合并赋值](#null%e5%90%88%e5%b9%b6%e8%b5%8b%e5%80%bc)
    - [非托管构造类型](#%e9%9d%9e%e6%89%98%e7%ae%a1%e6%9e%84%e9%80%a0%e7%b1%bb%e5%9e%8b)
    - [嵌套表达式中的 stackalloc](#%e5%b5%8c%e5%a5%97%e8%a1%a8%e8%be%be%e5%bc%8f%e4%b8%ad%e7%9a%84-stackalloc)
  

## C# 2.0版 - 2005

### 泛型

```cs
// Declare the generic class.
public class GenericList<T>
{
    public void Add(T input) { }
}
class TestGenericList
{
    private class ExampleClass { }
    static void Main()
    {
        // Declare a list of type int.
        GenericList<int> list1 = new GenericList<int>();
        list1.Add(1);

        // Declare a list of type string.
        GenericList<string> list2 = new GenericList<string>();
        list2.Add("");

        // Declare a list of type ExampleClass.
        GenericList<ExampleClass> list3 = new GenericList<ExampleClass>();
        list3.Add(new ExampleClass());
    }
}
```

### 分部类型


>拆分一个类、一个结构、一个接口或一个方法的定义到两个或更多的文件中是可能的。 每个源文件包含类型或方法定义的一部分，编译应用程序时将把所有部分组合起来。

```cs
public partial class Employee
{
    public void DoWork()
    {
    }
}

public partial class Employee
{
    public void GoToLunch()
    {
    }
}
```

### 匿名方法

```cs
Func<int, int, int> sum = delegate (int a, int b) { return a + b; };
Console.WriteLine(sum(3, 4));  // output: 7
```

### 可以为null的值类型

```cs
double? pi = 3.14;
char? letter = 'a';

int m2 = 10;
int? m = m2;

bool? flag = null;

// An array of a nullable type:
int?[] arr = new int?[10];
```

### 迭代器

```cs
static void Main()
{
    foreach (int number in SomeNumbers())
    {
        Console.Write(number.ToString() + " ");
    }
    // Output: 3 5 8
    Console.ReadKey();
}

public static System.Collections.IEnumerable SomeNumbers()
{
    yield return 3;
    yield return 5;
    yield return 8;
}
```

### 协变和逆变

>在 C# 中，协变和逆变能够实现数组类型、委托类型和泛型类型参数的隐式引用转换。 协变保留分配兼容性，逆变则与之相反。

```cs
// Assignment compatibility.   
string str = "test";  
// An object of a more derived type is assigned to an object of a less derived type.   
object obj = str;  
  
// Covariance.   
IEnumerable<string> strings = new List<string>();  
// An object that is instantiated with a more derived type argument   
// is assigned to an object instantiated with a less derived type argument.   
// Assignment compatibility is preserved.   
IEnumerable<object> objects = strings;  
  
// Contravariance.             
// Assume that the following method is in the class:   
// static void SetObject(object o) { }   
Action<object> actObject = SetObject;  
// An object that is instantiated with a less derived type argument   
// is assigned to an object instantiated with a more derived type argument.   
// Assignment compatibility is reversed.   
Action<string> actString = actObject;
```

## C# 3.0版 - 2007

### 自动实现的属性

```cs
// This class is mutable. Its data can be modified from
// outside the class.
class Customer
{
    // Auto-implemented properties for trivial get and set
    public double TotalPurchases { get; set; }
    public string Name { get; set; }
    public int CustomerID { get; set; }

    // Constructor
    public Customer(double purchases, string name, int ID)
    {
        TotalPurchases = purchases;
        Name = name;
        CustomerID = ID;
    }

    // Methods
    public string GetContactInfo() { return "ContactInfo"; }
    public string GetTransactionHistory() { return "History"; }

    // .. Additional methods, events, etc.
}

class Program
{
    static void Main()
    {
        // Intialize a new object.
        Customer cust1 = new Customer(4987.63, "Northwind", 90108);

        // Modify a property.
        cust1.TotalPurchases += 499.99;
    }
}
```

### 匿名类型

```cs
var v = new { Amount = 108, Message = "Hello" };  
  
// Rest the mouse pointer over v.Amount and v.Message in the following  
// statement to verify that their inferred types are int and n .  
Console.WriteLine(v.Amount + v.Message);
```

### 查询表达式（LINQ）

>我们通常认为 C# 版本的杀手锏是查询表达式，也就是语言集成查询 (LINQ)。
LINQ 的构造可以建立在更细微的视图检查表达式树、Lambda 表达式以及匿名类型的基础上。 不过无论如何 C# 3.0 都提出了革命性的概念。 C# 3.0 开始为 C# 转变为面向对象/函数式混合语言打下基础。
具体来说，你现在可以编写 SQL 样式的声明性查询对集合以及其他项目执行操作。 

### Lambda表达式

```cs
Func<int, int> square = x => x * x;
Console.WriteLine(square(5));
// Output:
// 25
```

### 表达式树

（还不是很理解）

### 扩展方法

>扩展方法使你能够向现有类型“添加”方法，而无需创建新的派生类型、重新编译或以其他方式修改原始类型。 

### var

```cs
var i = 10; // Implicitly typed.
int i = 10; // Explicitly typed.
```

### 分部方法

```cs
namespace PM
{
    partial class A
    {
        partial void OnSomethingHappened(string s);
    }

    // This part can be in a separate file.
    partial class A
    {
        // Comment out this method and the program
        // will still compile.
        partial void OnSomethingHappened(String s)
        {
            Console.WriteLine("Something happened: {0}", s);
        }
    }
}
```

### 对象和集合初始值设定项

```cs
public class Cat
{
    // Auto-implemented properties.
    public int Age { get; set; }
    public string Name { get; set; }

    public Cat()
    {
    }

    public Cat(string name)
    {
        this.Name = name;
    }
}
```

## C# 4.0版 - 2010

### 动态绑定

（这里文档里贴的链接是错的）

### 命名参数/可选参数

```cs
PrintOrderDetails(productName: "Red Mug", sellerName: "Gift Shop", orderNum: 31);
```

```cs
public void ExampleMethod(int required, string optionalstr = "default string",
    int optionalint = 10)
```

### 泛型中的协变和逆变

```cs
IEnumerable<Derived> d = new List<Derived>();
IEnumerable<Base> b = d;
```

```cs
Action<Base> b = (target) => { Console.WriteLine(target.GetType().Name); };
Action<Derived> d = b;
d(new Derived());
```

### 类型等效性和嵌入的互操作类型

目前理解成定义两个一样的类可以相互操作


## C# 5.0版 - 2012

### 异步编程

```cs
private DamageResult CalculateDamageDone()
{
    // Code omitted:
    //
    // Does an expensive calculation and returns
    // the result of that calculation.
}

calculateButton.Clicked += async (o, e) =>
{
    // This line will yield control to the UI while CalculateDamageDone()
    // performs its work.  The UI thread is free to perform other work.
    var damageResult = await Task.Run(() => CalculateDamageDone());
    DisplayDamage(damageResult);
};
```

### 调用方信息

```cs
public void DoProcessing()
{
    TraceMessage("Something happened.");
}

public void TraceMessage(string message,
        [System.Runtime.CompilerServices.CallerMemberName] string memberName = "",
        [System.Runtime.CompilerServices.CallerFilePath] string sourceFilePath = "",
        [System.Runtime.CompilerServices.CallerLineNumber] int sourceLineNumber = 0)
{
    System.Diagnostics.Trace.WriteLine("message: " + message);
    System.Diagnostics.Trace.WriteLine("member name: " + memberName);
    System.Diagnostics.Trace.WriteLine("source file path: " + sourceFilePath);
    System.Diagnostics.Trace.WriteLine("source line number: " + sourceLineNumber);
}

// Sample Output:
//  message: Something happened.
//  member name: DoProcessing
//  source file path: c:\Visual Studio Projects\CallerInfoCS\CallerInfoCS\Form1.cs
//  source line number: 31
```

## C# 6.0版 - 2015

### 静态导入

```cs
using static System.Math;
```

### 异常筛选器

```cs
public static async Task<string> MakeRequest()
{
    WebRequestHandler webRequestHandler = new WebRequestHandler();
    webRequestHandler.AllowAutoRedirect = false;
    using (HttpClient client = new HttpClient(webRequestHandler))
    {
        var stringTask = client.GetStringAsync("https://docs.microsoft.com/en-us/dotnet/about/");
        try
        {
            var responseText = await stringTask;
            return responseText;
        }
        catch (System.Net.Http.HttpRequestException e) when (e.Message.Contains("301"))
        {
            return "Site Moved";
        }
    }
}
```

### 自动初始化表达式

```cs
public ICollection<double> Grades { get; } = new List<double>();
```

### Expression-bodied 函数成员

```cs
public override string ToString() => $"{LastName}, {FirstName}";
```

### Null传播器

```cs
var first = person?.FirstName;
```

### 字符串内插

```cs
public string GetGradePointPercentage() =>
    $"Name: {LastName}, {FirstName}. G.P.A: {Grades.Average():F2}";
```

### `nameof`表达式

>nameof 表达式的计算结果为符号的名称。 每当需要变量、属性或成员字段的名称时，这是让工具正常运行的好办法。 nameof 的其中一个最常见的用途是提供引起异常的符号的名称：

```cs
if (IsNullOrWhiteSpace(lastName))
    throw new ArgumentException(message: "Cannot be blank", paramName: nameof(lastName));
```

### 索引初始值设定项

>使集合初始化更容易的另一个功能是对 Add 方法使用扩展方法 。 添加此功能的目的是进行 Visual Basic 的奇偶校验。 如果自定义集合类的方法具有通过语义方式添加新项的名称，则此功能非常有用。

## C# 7.0版 - 2017

### out变量

```cs
if (int.TryParse(input, out int result))
    Console.WriteLine(result);
else
    Console.WriteLine("Could not parse input");
```

### 元组和析构函数

```cs
(string Alpha, string Beta) namedLetters = ("a", "b");
Console.WriteLine($"{namedLetters.Alpha}, {namedLetters.Beta}");
```

析构函数应该类似C++中的析构函数，在实例回收时执行？

### 模式匹配

```cs
if (input is int count)
    sum += count;
```

### 本地函数

也可用lambda代替

```cs
public static IEnumerable<char> AlphabetSubset3(char start, char end)
{
    if (start < 'a' || start > 'z')
        throw new ArgumentOutOfRangeException(paramName: nameof(start), message: "start must be a letter");
    if (end < 'a' || end > 'z')
        throw new ArgumentOutOfRangeException(paramName: nameof(end), message: "end must be a letter");

    if (end <= start)
        throw new ArgumentException($"{nameof(end)} must be greater than {nameof(start)}");

    return alphabetSubsetImplementation();

    IEnumerable<char> alphabetSubsetImplementation()
    {
        for (var c = start; c < end; c++)
            yield return c;
    }
}
```

### 更多的expression-bodied成员

```cs
// Expression-bodied constructor
public ExpressionMembersExample(string label) => this.Label = label;

// Expression-bodied finalizer
~ExpressionMembersExample() => Console.Error.WriteLine("Finalized!");

private string label;

// Expression-bodied get / set accessors.
public string Label
{
    get => label;
    set => this.label = value ?? "Default label";
}
```

### Ref 局部变量和返回结果

>此功能允许使用并返回对变量的引用的算法，这些变量在其他位置定义。 一个示例是使用大型矩阵并查找具有某些特征的单个位置。 

```cs
public static ref int Find(int[,] matrix, Func<int, bool> predicate)
{
    for (int i = 0; i < matrix.GetLength(0); i++)
        for (int j = 0; j < matrix.GetLength(1); j++)
            if (predicate(matrix[i, j]))
                return ref matrix[i, j];
    throw new InvalidOperationException("Not found");
}
```

```cs
ref var item = ref MatrixSearch.Find(matrix, (val) => val == 42);
Console.WriteLine(item);
item = 24;
Console.WriteLine(matrix[4, 2]);
```

### 弃元
### 二进制文本和数字分隔符
### 引发表达式


## C# 8.0版 - 2019

### Readonly 成员

```cs
public readonly override string ToString() =>
    $"({X}, {Y}) is {Distance} from the origin";
```

### 默认接口方法
### 在更多位置中使用更多模式

#### switch表达式

```cs
public static RGBColor FromRainbow(Rainbow colorBand) =>
    colorBand switch
    {
        Rainbow.Red    => new RGBColor(0xFF, 0x00, 0x00),
        Rainbow.Orange => new RGBColor(0xFF, 0x7F, 0x00),
        Rainbow.Yellow => new RGBColor(0xFF, 0xFF, 0x00),
        Rainbow.Green  => new RGBColor(0x00, 0xFF, 0x00),
        Rainbow.Blue   => new RGBColor(0x00, 0x00, 0xFF),
        Rainbow.Indigo => new RGBColor(0x4B, 0x00, 0x82),
        Rainbow.Violet => new RGBColor(0x94, 0x00, 0xD3),
        _              => throw new ArgumentException(message: "invalid enum value", paramName: nameof(colorBand)),
    };
```

#### 属性模式

```cs
public static decimal ComputeSalesTax(Address location, decimal salePrice) =>
    location switch
    {
        { State: "WA" } => salePrice * 0.06M,
        { State: "MN" } => salePrice * 0.75M,
        { State: "MI" } => salePrice * 0.05M,
        // other cases removed for brevity...
        _ => 0M
    };
```

#### 元组模式

```cs
public static string RockPaperScissors(string first, string second)
    => (first, second) switch
    {
        ("rock", "paper") => "rock is covered by paper. Paper wins.",
        ("rock", "scissors") => "rock breaks scissors. Rock wins.",
        ("paper", "rock") => "paper covers rock. Paper wins.",
        ("paper", "scissors") => "paper is cut by scissors. Scissors wins.",
        ("scissors", "rock") => "scissors is broken by rock. Rock wins.",
        ("scissors", "paper") => "scissors cuts paper. Scissors wins.",
        (_, _) => "tie"
    };
```

#### 位置模式

```cs
static Quadrant GetQuadrant(Point point) => point switch
{
    (0, 0) => Quadrant.Origin,
    var (x, y) when x > 0 && y > 0 => Quadrant.One,
    var (x, y) when x < 0 && y > 0 => Quadrant.Two,
    var (x, y) when x < 0 && y < 0 => Quadrant.Three,
    var (x, y) when x > 0 && y < 0 => Quadrant.Four,
    var (_, _) => Quadrant.OnBorder,
    _ => Quadrant.Unknown
};
```

### using声明

```cs
static int WriteLinesToFile(IEnumerable<string> lines)
{
    using var file = new System.IO.StreamWriter("WriteLines2.txt");
    // Notice how we declare skippedLines after the using statement.
    int skippedLines = 0;
    foreach (string line in lines)
    {
        if (!line.Contains("Second"))
        {
            file.WriteLine(line);
        }
        else
        {
            skippedLines++;
        }
    }
    // Notice how skippedLines is in scope here.
    return skippedLines;
    // file is disposed here
}
```

### 静态本地函数

```cs
int M()
{
    int y = 5;
    int x = 7;
    return Add(x, y);

    static int Add(int left, int right) => left + right;
}
```

### 异步流

```cs
public static async System.Collections.Generic.IAsyncEnumerable<int> GenerateSequence()
{
    for (int i = 0; i < 20; i++)
    {
        await Task.Delay(100);
        yield return i;
    }
}
```

### 索引和范围

感觉类似python中的切片器，`-`用`^`代替了

```cs
var words = new string[]
{
                // index from start    index from end
    "The",      // 0                   ^9
    "quick",    // 1                   ^8
    "brown",    // 2                   ^7
    "fox",      // 3                   ^6
    "jumped",   // 4                   ^5
    "over",     // 5                   ^4
    "the",      // 6                   ^3
    "lazy",     // 7                   ^2
    "dog"       // 8                   ^1
};              // 9 (or words.Length) ^0

var quickBrownFox = words[1..4];
var lazyDog = words[^2..^0];
var allWords = words[..]; // contains "The" through "dog".
var firstPhrase = words[..4]; // contains "The" through "fox"
var lastPhrase = words[6..]; // contains "the", "lazy" and "dog"
```

### Null合并赋值

```cs
List<int> numbers = null;
int? i = null;

numbers ??= new List<int>();
numbers.Add(i ??= 17);
numbers.Add(i ??= 20);

Console.WriteLine(string.Join(" ", numbers));  // output: 17 17
Console.WriteLine(i);  // output: 17
```

### 非托管构造类型

>与任何非托管类型一样，可以创建指向此类型的变量的指针，或针对此类型的实例在堆栈上分配内存块

```cs
Span<Coords<int>> coordinates = stackalloc[]
{
    new Coords<int> { X = 0, Y = 0 },
    new Coords<int> { X = 0, Y = 3 },
    new Coords<int> { X = 4, Y = 0 }
};
```

### 嵌套表达式中的 stackalloc

```cs
Span<int> numbers = stackalloc[] { 1, 2, 3, 4, 5, 6 };
var ind = numbers.IndexOfAny(stackalloc[] { 2, 4, 6 ,8 });
Console.WriteLine(ind);  // output: 1
```