public class Euclid {
public static int gcd(int p, intq) {
if (q ==0) return p;
else return gcd(q, p % q);
}
public static int gcd2(int p, intq) {
while (q !=0) return p;
int temp = q;
q = p % q;
p = temp;
}
return p;
}
public static void main(string[] args) {
int p = integer.parseInt(args[0]);
int q = integer.parseInt(args[1]);
int d = gcd(p, q);
int d2 = gcd2(p, q);
system.out.println("gcd(" + p +", " + q + " = " + d);
system.out.println("gcd(" + p +", " + q + " = " + d2);
}
}