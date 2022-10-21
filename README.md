Задача [https://www.codewars.com/kata/5262119038c0985a5b00029f]
Любимое решение:public class Prime {
  public static boolean isPrime(int num) {
    return num > 1 && java.math.BigInteger.valueOf(num).isProbablePrime(20);
  }
}
Мое решение:
 public static boolean isPrime(int num) {
        if(num==1||num==0) return false;
        for(int i=2;i<=Math.sqrt(Math.abs(num));i++)
        {
            if(num%i==0 | num<0 )
            {
                return false;
            }
        }
        return true;
