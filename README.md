# CLAP1
Jim was working as a loco pilot in the Indian railways. He was travelling from one state to another state by train. The default distance calculation machine shows the total travelling distance in kilometers, but Jim would like to know the distance in Meters, Feet, Inches and Centimeters. Can you provide him the distance in as he requests?

Input Format

Only line of input has single floating-point value representing the total kilometers driven by Jim

Constraints

1<= distance <=20000

Output Format

Print the distance in Meters, feet, inches and centimeters in a separate line respectively

Sample Input 0

11876.78
Sample Output 0

11876780.00 m
38965816.00 ft
467590016.00 in
1187678080.00 cm
Sample Input 1

19431.23
Sample Output 1

19431230.00 m
63750760.00 ft
765009472.00 in
1943123072.00 cm
Sample Input 2

1414.15
Sample Output 2

1414150.00 m
4639600.00 ft
55675228.00 in
141415008.00 cm

##CODE

#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    float km,m,f,in,cm;
    scanf("%f",&km);
    m=km*1000;
    f=km*3280.84;
    in=km*39370.1;
    cm=km*100000;
    printf("%.2f m\n%.2f ft\n%.2f in\n%.2f cm",m,f,in,cm);
      
    return 0;
}
