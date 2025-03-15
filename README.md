# C11
Structure in structure #include<stdio.h>
struct date{ 
int day,month,year;
};
struct student {
char name[50];
int rollno;
struct date dob;
};
int main()
{
struct student s1={"meghana",20,{9,8,2004}};
printf("student  name is %s\n",s1.name);
printf ("age:%d\n",s1.rollno);
printf ("date  of birth %2d-%02d-%02d\n",s1.dob.day,s1.dob.month,s1.dob.year);
return 0 ;
}
