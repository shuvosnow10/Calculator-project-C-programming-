# Calculator-project-C-programming-
This is small beginner level C programming project . it's a normal calculator program .

#include <stdio.h>
#include <math.h>

int main()
{

  char oparetor;
  double num1;
  double num2;
  double result;
  printf("ENTER ANY OPARETOR:->");
  scanf("%C", &oparetor);

  printf("Enter number1 to calculate= ");
  scanf("%lf", &num1);
  printf("Enter number2 to calculate= ");
  scanf("%lf", &num2);
  switch (oparetor)
  {
  case '^':
    result = pow(num1, num2);
    printf("The result(for power)=%lf", result);
    break;
  case '~':
    result = sqrt(num1);
    printf("\nThe value of root=%lf", result);
    break;
  case '+':
    result = num1 + num2;
    printf("The result=%lf\n", result);
    break;
  case '-':
    result = num1 - num2;
    printf("The result%lf", result);
    break;
  case '*':
    result = num1 * num2;
    printf("The result =%lf", result);
    break;
  case '/':
    result = num1 / num2;
    printf("The result=%lf", result);
    break;
  default:
    printf("\n%c Is not a valued operator ", oparetor);
  }

  return 0;
}
