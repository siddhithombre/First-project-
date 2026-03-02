#include <stdio.h>

int main()
{
    float a, b, c;
    float total, dis, dis_amount, tax, final_amount;

    printf("Enter price of first item = ");
    scanf("%f", &a);

    printf("Enter price of second item = ");
    scanf("%f", &b);

    printf("Enter price of third item = ");
    scanf("%f", &c);

    total = a + b + c;
    dis = total * 0.02;
    dis_amount = total - dis;
    tax = dis_amount * 0.05;
    final_amount = dis_amount + tax;

    printf("\n------ TOTAL BILL ------\n");
    printf("Total Amount = %f\n", total);
    printf("Discount (2%%) = %f\n", dis);
    printf("Discounted Amount = %f\n"dis_amount);
    printf("Tax (5%%) = %f\n", tax);
    printf("Final Payable Amount = %f\n",final_amount);

    return 0;
}