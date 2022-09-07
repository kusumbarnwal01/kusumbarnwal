Kusum Barnwal
Reg. No.: - 12105597
Student, Department of Computer Applications,
Lovely Professional University
Email: - kusumbarnwal135@gmail.com
Mob No.: - 7365863124

<!-- Code -->

import java.util.*;

class product{
    String name;
    product(String name)
    {
        this.name=name;
    }

    void get()
    {
        System.out.println(name);
    }
}

class gst{
    int g;
    gst(int g)
    {
        this.g = g;
    }

    void get()
    {
        System.out.println(g);
    }
}

class quantity{
    int q;
    
    quantity(int q)
    {
        
        this.q  = q;
    }

   void get()
    {
        System.out.println(q);
    }
}

class price{
    int p;
    static int sum=0;
    price(int p)
    {
        sum=sum+p;
        this.p  = p;
    }

    void get()
    {
        System.out.println(p);
    }

    void totalp()
    {
        System.out.println("total price" + sum);
    }
}



class Main{
    public static void main(String args[])
    {
       product p = new product("Leather Wallet");
       product p1 = new product("Umbrella");
       product p2 = new product("Cigarette");
       product p3 = new product("Honey");

       gst g = new gst(18);
       gst g1 = new gst(12);
       gst g2 = new gst(28);
       gst g3 = new gst(0);

       quantity q = new quantity(1);
       quantity q1 = new quantity(2);
       quantity q2 = new quantity(3);
       quantity q3 = new quantity(4);
       
       price c = new price(1100);
       price c1 = new price(900);
       price c2 = new price(200);
       price c3 = new price(100);
       
       p.get();
       p1.get();
       p2.get();
       p3.get();
       System.out.println();

       g.get();
       g1.get();
       g2.get();
       g3.get();
       System.out.println();

       q.get();
       q1.get();
       q2.get();
       q3.get();
       System.out.println();

       c.get();
       c1.get();
       c2.get();
       c3.get();
       System.out.println();
       c.totalp();
       System.out.println();
    }
}
