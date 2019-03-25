# Objek-parameter

class kotak1 {
    double panjang ;
    double lebar;
    double tinggi;
    
    kotak1 (double p, double l, double t){
    panjang=p;
    lebar = l;
    tinggi=t;
    }
    
    double hitungVolume (){
    return (panjang*lebar*tinggi);
    }
    
    //mendefinisikan method dengan parameter objek kotak
    boolean sama (kotak1 k){
    if ((k.panjang==this.panjang)&&
        (k.lebar==this.lebar)&&
        (k.tinggi==this.tinggi)){
    return true;}
    else{
    return false;
        }
    }
}
public class demoOverload2 {
    public static void main (String[]args){
    kotak1 k1,k2,k3,k4;
    k1=new kotak1(4,3,2);
    k2=new kotak1(6,5,4);
    k3=new kotak1(4,3,2);
    k4=new kotak1(6,5,4);
    
    
    System.out.println ("k1==k2 : "+k1.sama(k2));
    System.out.println ("k1==k3 : "+k1.sama(k3));
    System.out.println ("k1==k4 : "+k1.sama(k4));
    }
    
}
