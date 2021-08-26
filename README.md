# employee-s-details
This c program prints the employees details like name,age, phone number, salary
#include <stdio.h>
#include <stdlib.h>
 
typedef struct{
 
    char name[30];
    int Age;
    int phonenumber;
    int salary;
 
} Employee;
 
int main()
{
    int i, n=2;
 
    Employee employees[n];
 
    //Taking each employee detail as input
 
    printf("Enter %d Employee Details \n \n",n);
    for(i=0; i<n; i++){
 
        printf("Employee %d:- \n",i+1);
        //Name
        printf("Name: ");
        scanf("%s",employees[i].name);
        //ID
        printf("Age: ");
        scanf("%d",&employees[i].Age);
        printf("phonenumber:");
        scanf("%d",& employees [i]. phonenumber);
        printf("Salary: ");
        scanf("%d",&employees[i].salary);
 
        printf("\n");
    }
 
    //Displaying Employee details
 
    printf("-------------- All Employees Details ---------------\n");
 
    for(i=0; i<n; i++){
 
        printf("Name \t: ");
        printf("%s \n",employees[i].name);
 
        printf("Age \t: ");
        printf("%d \n",employees[i].Age);
       printf("phonenumber\t:");
       printf("%d\n", employees [i].phonenumber);
        printf("Salary \t: ");
        printf("%d \n",employees[i].salary);
 
        printf("\n");
    }
 
    return 0;
 
}
