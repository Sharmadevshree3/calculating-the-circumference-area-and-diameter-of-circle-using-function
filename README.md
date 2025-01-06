# calculating-the-circumference-area-and-diameter-of-circle-using-function
#include <stdio.h>
#include <math.h>
float Diameter(double radius);
float Circumference(double radius);
float Area(double radius);


int main() 
{
    float radius, dia, circ, area;
    
    
    printf("Enter radius of circle: ");
    scanf("%f", &radius);
    
    dia  = Diameter(radius);      
    circ = Circumference(radius);  
    area = Area(radius);           
    
    printf("Diameter of the circle = %.2f units\n", dia);
    printf("Circumference of the circle = %.2f units\n", circ);
    printf("Area of the circle = %.2f sq. units", area);
    
    return 0;
}



float Diameter(double radius) 
{
    return (2 * radius);
}



float Circumference(double radius) 
{
    return (2 * M_PI * radius); 
}



float Area(double radius)
{
    return (M_PI * radius * radius); 
}
