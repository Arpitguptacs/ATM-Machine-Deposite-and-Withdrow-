# ATM-Machine-Deposite-and-Withdrow-
Working process of ATM machine 

#include <stdio.h>
#include <stdbool.h>




void p_amount(int amount,int p){
    
    
    int p_amount;
    int new_amount;

   switch (p){
   case 1234:
    p_amount =  50000;
    new_amount = p_amount+amount;
   printf("Your  account has previus balence was = %d \nNow present account balence is %d", p_amount,new_amount);
   break;

   case 5678:
    p_amount =  580000;
    new_amount = p_amount+amount;
   printf("Your  account  has previus balence was = %d \nNow present account balence is %d", p_amount,new_amount);
   break;

   case 9101112:
    p_amount =  4550000;
    new_amount = p_amount+amount;
   printf("Your  account  has previus balence was = %d \nNow present account balence is %d", p_amount,new_amount);
   break;

   case 13141516:
    p_amount =  3650000;
    new_amount = p_amount+amount;
   printf("Your  account  has previus balence was = %d \nNow present account balence is %d", p_amount,new_amount);
   break;

   case 17181920:
    p_amount =  59580000;
    new_amount = p_amount+amount;
   printf("Your  account  has previus balence was = %d \nNow present account balence is %d", p_amount,new_amount);
   break;
   }

}

void Diposite(int pass){
    int amount;
 switch(pass){
    case 1234: 
    printf("Enter diposite amount\n");
    scanf("%d",&amount);
    p_amount(amount,pass);
    break;

    case 5678: 
    printf("Enter diposite amount\n");
    scanf("%d",&amount);
    p_amount(amount,pass);
    break;

    case 9101112: 
    printf("Enter diposite amount\n");
    scanf("%d",&amount);
    p_amount(amount,pass);
    break;

    case 13141516: 
    printf("Enter diposite amount\n");
    scanf("%d",&amount);
    p_amount(amount,pass);
    break;

    case 17181920: 
    printf("Enter diposite amount\n");
    scanf("%d",&amount);
    p_amount(amount,pass);
    break;
    
    default: printf("Invaled Acount\n");


 }

}

int main(){
    
    // int total_Ac[5] = {1250,1542,13625,4724,468145};
    
    printf("\n_____WELCOME TO INDIAN BANK_______\n");
        
    int ac_n;
    printf("\nEnter Account number\n");
    scanf("%d",&ac_n);

    int pass;
    printf("\nEnter pass key\n");
    scanf("%d",&pass);

    printf("1.Deposite Amount\n");
    printf("2.Withdrow Amount\n");

    short int  flag;
    scanf("%hd",&flag);

    if(flag==1){ 
        
        Diposite(pass); 
    }else{

    }

    
    return 0;
}
