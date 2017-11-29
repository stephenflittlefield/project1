# Project 1

## Bubble Sort

This is a program to help sort random numbers into a list of numbers in numerical order.

## How to Begin:

After you have installed Java and Netbeans. Copy the code into a Netbeans project.

package sort;

import java.math.*;

public class Sort {

 
    public static void main(String[] args) {
        
        int[] n = new int[10];
        for (int i = 0; i<10; i++){
            n[i] = (int)(Math.random()*100)+1;
        }
        System.out.println("Unsorted list!");
        for (int i = 0; i<10; i++){
            System.out.print(n[i] + ", ");
        }    
        System.out.println("\n");
        bubbleSort(n);
        
        System.out.println("Sorted list!");
        for (int i = 0; i<10; i++){
            System.out.print(n[i] + ", ");
        }
    
    }    
          
    
    
    private static void bubbleSort(int[] n){
        boolean done = false;
        while (!done){
          done = true;
          for (int i=0; i < n.length-1; ++i){
            if (n[i] > n[i+1]){
                int num = n[i];
                n[i] = n[i+1];
                n[i+1] = num;
                done = false;
            }
          }   
        }
         
    }  



Prerequisites

The program is written using Java code and will need Java and NetBeans to run the Bubble Sort.

Java SE Download:www.oracle.com

Above is the link to the official Java SE download page from Oracle. When you are ready to install Java on your personal computer, open a link and be sure to select "JDK" instead of "JRE".  Clicking the "JRE" button will take you to another page, in which you will be asked to accept Oracle's licensing agreement.  Next, download the version of the JDK which corresponds to your operating system; for example, if you are running a 64-bit version of Windows (which you probably are if you have a fairly recent computer), click the "Windows x64" link to download the 64-bit installer.  If you have a 32-bit computer, download the "Windows x86" version instead.

NetBeans IDE Download:https://netbeans.org

Above is the link to the official NetBeans download page.  When you are ready to install NetBeans on your own computer, open this link.  I recommend installing the "Java EE" version of NetBeans; it will add Web application functionality that you might find useful in a future class.

As an alternative, you can follow the Java download link and download the JDK and NetBeans in a single package.  You should see this option when you follow the link given above.

**Up and Running**

Open Netbeans IDE

Left click on the **File** tab in the tool bar

Hover over the **New Project** and select it

When the menu box appears, click next

The second menu box will appear. In the Title box title your project "Sort" and then hit "Finish"

Delete all the content in the source window

Copy and paste the above code into the source window

Save and compile the project using the **Hammer and Broom** icon

Run the project using the **Green Arrow** icon






Author

    S.Littlefield

See also the list of contributors who participated in this project.
License

This project is licensed under the YadaYada License - see the LICENSE.md file for details
Acknowledgments

    Hat tip to anyone who's code was used
    Inspiration
    etc
