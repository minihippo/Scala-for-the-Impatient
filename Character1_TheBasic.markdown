# The Basics

### Exercise

1. ans: 
  ~~~Shell
  scala> 3.
  ~~~

  ~~~shell
  !=   >             floatValue      isValidInt     to               toRadians
  %    >=            floor           isValidLong    toBinaryString   toShort
  &    >>            getClass        isValidShort   toByte           unary_+
  *    >>>           intValue        isWhole        toChar           unary_-
  +    ^             isInfinite      longValue      toDegrees        unary_~
  -    abs           isInfinity      max            toDouble         underlying
  /    byteValue     isNaN           min            toFloat          until
  <    ceil          isNegInfinity   round          toHexString      |
  <<   compare       isPosInfinity   self           toInt
  <=   compareTo     isValidByte     shortValue     toLong
  ==   doubleValue   isValidChar     signum         toOctalString
  ~~~

2. ans:
   ~~~shell
   scala> import scala.math._
   import scala.math._

   scala> val ans = sqrt(3)
   ans: Double = 1.7320508075688772
   ~~~

   ~~~shell
   scala> val res = 3-pow(ans,2)
   res: Double = 4.440892098500626E-16
   ~~~

3. val

   ~~~shell
   scala> 1
   res0: Int = 1

   scala> res0 = 2
   <console>:12: error: reassignment to val
   ~~~

4. class StringOps [scala.collection.immutable](http://www.scala-lang.org/api/2.12.3/scala/collection/immutable/StringOps.html)
   ~~~shell
   scala> "crazy"*3
   res1: String = crazycrazycrazy
   ~~~

5. class RichInt [scala.runtime](http://www.scala-lang.org/api/2.12.3/scala/runtime/RichInt.html)

   ~~~shell
   scala> 10 max 2
   res3: Int = 10
   ~~~

6. ans:
   ~~~shell
   scala> val ans:BigInt = 2
   ans: scala.math.BigInt = 2

   scala> ans.pow(1024)
   res2: scala.math.BigInt = 179769313486231590772930519078902473361797697894230657273430081157732675805500963132708477322407536021120113879871393357658789768814416622492847430639474124377767893424865485276302219601246094119453082952085005768838150682342462881473913110540827237163350510684586298239947245938479716304835356329624224137216
   ~~~

7. ans:
   ~~~shell
   scala> import scala.util.Random
   import scala.util.Random

   scala> import scala.math.BigInt._
   import scala.math.BigInt._

   scala> probablePrime(100,Random)
   res5: scala.math.BigInt = 1094141631787021174802643788977
   ~~~

8. ans:
   ~~~shell
   scala> probablePrime(100,Random).toString(36)
   res6: String = 325q071gt9nrizr89akt
   ~~~

9. ans:
   ~~~shell
   scala> "123".head
   res10: Char = 1

   scala> "123".last
   res13: Char = 3
   ~~~

10. ans: 
   ~~~shell
   scala> "string".drop(3)
   res14: String = ing

   scala> "string".take(3)
   res15: String = str

   scala> "string".takeRight(2)
   res16: String = ng

   scala> "string".dropRight(2)
   res17: String = stri
   ~~~
