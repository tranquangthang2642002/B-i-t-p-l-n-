#include<stdio.h>
#include<iostream>
#include<conio.h>
#include <stdlib.h>


 struct Giohang {
  	char tenkhachhang[30];
  	char diachi[50];
  	int sosanpham;
  	
  	  struct sp_stdssp;
	     char tensp[30];
	     int gia;
	     int soluong;
	 };
	 typedef Giohang GH;
	  void nhap (GH &gh);
	  void nhapN (GH a[],int n);
	  
	   void nhap (GH &gh){
	   printf("\nNhap ten san pham:");
	   fflush(stdin);
	   scanf("%d",&gh.tensp);
	   printf("\nNhap gia:");
	   scanf("%f",&gh.gia);
	   printf("\nNhap so luong:");
	   scanf("%d",&gh.soluong);
	   printf("\n");
	   }
	   void nhapN (GH a[],int n){
	   	for (int i=0;i<n;i++){
	   		printf("Nhap so san pham:%d",i+1);
	   		nhap (a[i]);
		   }
	   }
	   
int main(){
	GH a[20];
	int n;
	int key;
	do{
		printf ("nhap so luong san pham: ");
		scanf ("%d",&n);
	}while (n <= 0);


   
	printf("======================================================\n");
	printf("                       MENU                           \n");
	printf("======================================================\n");
	printf("                   ***1.Gio hang***                   \n");
	printf("                   ***2.Chon hang***                  \n");
	printf("                   ***3.Xem chi tiet gio hang***      \n");
	printf("                   ***4.Loai bo mot mat hang***       \n");
	printf("                   ***5Thoat***                       \n");
    printf("______________________________________________________\n"); 
    printf("                   Lua cho cua ban                    \n");
    
    scanf("%d",key);  
    
    switch (key){
    	case 1:
             printf("\nNhap ten khach hang:%d");
             nhapN (a,n);
			 printf("\nNhap dia chi:%d");
			 nhapN (a,n);
			 printf("\nSo luong san pham:0");
		     getch();
			 break;
		case 2:
		   printf ("\nban da chon in phieu thanh toan.\n");
			break;
			
	    case 3:
	    	printf("______________________________________________\n");
	    	printf("|STT   |   Ten sam pham   |  Gia   | So luong|\n");
	    	printf("______________________________________________\n");
	    	printf("|  1   |     Ca chua      | 3000   |      3  |\n");
	    	printf("______________________________________________\n");
	    	printf("|  2   | Kem socola       |  5500  |     10  |\n");
	    	printf("______________________________________________\n");
	    	printf("|  3   |  Vo hoc sinh     |  4000  |    20   |\n");
	    	printf("______________________________________________\n");
	    	getch();
	    	break;
	    	
		}
					
	}
   
  	      

  
  	     
  	         
  	     
