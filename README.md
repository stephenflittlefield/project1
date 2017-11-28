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

A step by step series of examples that tell you have to get a development env running

Say what the step will be

Give the example

And repeat

until finished

End with an example of getting some data out of the system or using it for a little demo
Running the tests

Explain how to run the automated tests for this system
Break down into end to end tests

Explain what these tests test and why

Give an example

And coding style tests

Explain what these tests test and why

Give an example

Deployment

Add additional notes about how to deploy this on a live system
Built With

    Dropwizard - The web framework used
    Maven - Dependency Management
    ROME - Used to generate RSS Feeds

Contributing

Please read CONTRIBUTING.md for details on our code of conduct, and the process for submitting pull requests to us.
Versioning

We use SemVer for versioning. For the versions available, see the tags on this repository.
Authors

    Billie Thompson - Initial work - PurpleBooth

See also the list of contributors who participated in this project.
License

This project is licensed under the MIT License - see the LICENSE.md file for details
Acknowledgments

    Hat tip to anyone who's code was used
    Inspiration
    etc
