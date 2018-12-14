# #include <stdio.h>
#include <math.h>
void main() {

	double a, b, c, p, q;
	printf(" insetrt the equation to.. in the next pattern:(a,b,c)\n");
	scanf_s("%f,%f,%f", &a, &b, &c);
	//////////p = -b / 2 * a;
		////////q = sqrt(b*b - 4 * a*c) / 2 * a;
	if (a != 0) {
		//dis = b*b - 4 * a*c;
		if (b*b - 4 * a*c > 0) {
			printf("the answer is: x1=%.9lf and x2=%lf", (-b + sqrt(b*b - 4 * a*c)) / 2 * a, (-b - sqrt(b*b - 4 * a*c)) / 2 * a);
			/*x1 = (-b + sqrt(dis)) / 2a;
			x2 = (-b - sqrt(dis)) / 2a;*/
		}
		else if (b*b - 4 * a*c == 0) {  //else if (dis == 0){
			printf("x1 =%lf", -b / 2 * a);	//x1=-b/2a}
		}
		else {
			printf("x1=%lf  x2=%lf i", -b / 2 * a, sqrt(b*b - 4 * a*c) / 2 * a);
			//printf("x1=%lf \n, x2=lf i\n", p, q);

		}
	}

	else {
		if (b != 0) {
			printf("x1=%lf\n", -c / b);
		}
		else {
			if (c == 0)printf("any x");
			else printf("no answer");
		}
	}
	system("pause");

}
