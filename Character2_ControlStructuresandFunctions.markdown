# Control Structures and Functions

#### Exercises

1. ans:
   ~~~shell
   scala> def ans(arg:Int)= 
   	if (arg > 0 ) 
   		1 
   	else if(arg < 0) 
   		-1 
   	else 
   		0
   ans: (arg: Int)Int

   scala> ans(1)
   res1: Int = 1

   scala> ans(-1)
   res2: Int = -1

   scala> ans(0)
   res3: Int = 0
   ~~~

2. 空值() unit

3. val x : Unit

4. ans:
   ~~~shell
   scala> for (i <- (0 to 10).reverse) System.out.println(i)
   10
   9
   8
   7
   6
   5
   4
   3
   2
   1
   0
   ~~~

5. ans:
   ~~~shell
   scala> def countdown(n:Int) = 
   	for (i <- (0 to n).reverse) 
   		System.out.println(i)
   countdown: (n: Int)Unit

   scala> countdown(4)
   4
   3
   2
   1
   0
   ~~~

6. ans:
   ~~~shell
   scala> def ans(string : String) : Long = {
   	var mul = 1L; 
   	for (ele <- string) 
   		mul *= ele.toLong; mul}
   ans: (string: String)Long

   scala> ans("Hello")
   res1: Long = 9415087488
   ~~~

7. ans:
   ~~~shell
   scala> def ans(string : String) : Long = {
   	var mul = 1L; 
   	string.foreach(mul *= _.toLong); mul}
   ans: (string: String)Long

   scala> ans("Hello")
   res2: Long = 9415087488
   ~~~

8. the same with 7

9. ans:
   ~~~shell
   scala> def ans(args: String) : Long = { 
   	if (args.length == 1) 
   		args.head.toLong 
   	else 
   		args.head.toLong*ans(args.tail)};
   ans: (args: String)Long

   scala> ans("Hello")
   res4: Long = 9415087488
   ~~~

10. ans: 
    ~~~shell
    scala> def ans(x:Double,n:Int) : Double = {
         | if (n == 0) 1L
         | else if (n > 0 && n%2 == 1) x*ans(x,n-1)
         | else if (n > 0 && n%2 == 0) ans(x,n/2)*ans(x,n/2)
         | else 1/ans(x,-n)
         | }
    ans: (x: Double, n: Int)Double

    scala> ans(2,-2)
    res5: Double = 0.25

    scala> ans(2,3)
    res6: Double = 8.0

    scala> ans(2,2)
    res7: Double = 4.0
    ~~~
