# Factorial-program-in-C

# Apporach-1
# C program to implement the above approach
#include <stdio.h>
# Function to find factorial of given number
unsigned int factorial(unsigned int n)
{
	int result = 1, i;
	for (i = 2; i <= n; i++) {
		result *= i;
	}

	return result;
}
# Driver code
int main()
{
	int num = 5;
	printf("Factorial of %d is %d", num, factorial(num));
	return 0

 # Apporach-2
 
 #include <stdio.h>
int main() {
    int n, i;
    unsigned long long fact = 1;
    printf("Enter an integer: ");
    scanf("%d", &n);

    //shows error if the user enters a negative integer
    if (n < 0)
        printf("Error! Factorial of a negative number doesn't exist.");
    else {
        for (i = 1; i <= n; ++i) {
            fact *= i;
        }
        printf("Factorial of %d = %llu", n, fact);
    }

    return;
    
# Apporach-3
# Factorial program using loop
#include<stdio.h>  
int main()    
{    
 int i,fact=1,number;    
 printf("Enter a number: ");    
  scanf("%d",&number);    
    for(i=1;i<=number;i++){    
      fact=fact*i;    
  }    
  printf("Factorial of %d is: %d",number,fact);    
return 0;  
} 

# Apporach-4

# factorial Using Recursion Method

#include<stdio.h>  
  
long factorial(int n)  
{  
  if (n == 0)  
    return 1;  
  else  
    return(n * factorial(n-1));  
}  
   
void main()  
{  
  int number;  
  long fact;  
  printf("Enter a number: ");  
  scanf("%d", &number);   
   
  fact = factorial(number);  
  printf("Factorial of %d is %ld\n", number, fact);  
  return 0;  
}  


# Apporach-5

# Calculate the factorial program
#include <stdio.h>  

int  main(){
  int i, f = 1, num;

  printf("Input the number : ");  
  scanf("%d", &num);  

  for(i = 1; i <= num; i++)  
      f = f * i;  // Calculate factorial.

  printf("The Factorial of %d is: %d\n", num, f);  
   return 0;  
}

