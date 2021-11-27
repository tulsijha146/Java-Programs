/* Write a method in java which can do both sum or multiply of 2 numbers based on parameters passed to method*/

class summutiply
{
public void sum(int a,int b)
{
int add=a+b;
System.out.println("Sum of "+a+" and "+b+" is "+add);
}
public void multiply(int a,int b)
{
int mul=a*b;
System.out.println("Multiplication of "+a+" and "+b+" is "+mul);
}
public static void main(String[] args)
{
summutiply obj1=new summutiply();
int a,b;
obj1.sum(3,5);
obj1.multiply(3,5);
}
}


/*Write  function to find 2 smallest number from an array*/


class smallestnum
{
  public void smallest(int arr[],int len)
  {
    int temp;
    for(int i=0;i<len;i++)
    {
      for(int j=i+1;j<len;j++)
      {
        if(arr[i]>arr[j])
        {
          temp=arr[i];
          arr[i]=arr[j];
          arr[j]=temp;
        }
      }
    }
    System.out.println("Smallest num="+arr[1]);
  }
  public static void main(String args[])
  {
    smallestnum obj=new smallestnum();
    int arr[]={40,6,80,56,73,21,5}; 
    obj.smallest(arr,arr.length);
  }
}
