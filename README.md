TotalSales
==========
public class TotalSales
{
   public static void main(String[] args)
   {
      
      java.util.Scanner keyboard = new java.util.Scanner(System.in);
   
      int days;
      double sales, totalSales;
      String input;
      
      //get number of days
      System.out.println("For how many days " +
                        "do you have sales figures?");
      days = keyboard.nextInt();
      
      //set accumulator to 0.
      totalSales = 0.0;
      
      //get the sales figures and calculate a running total.
      for (int count = 1; count <= days; count++)
      {
         System.out.println("Enter the sales " +
                        "for day " + count + ":");
         sales = keyboard.nextDouble();
         totalSales += sales; //add sales to totalSales
      }
      
      //display total sales.
      System.out.printf("The total sales are $" +
                        "%.2f\n", totalSales);
                        
      System.exit(0);
      
     }
     
}
      
