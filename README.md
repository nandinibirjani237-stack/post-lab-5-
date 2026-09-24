# post-lab-5-
# lab-5
#task 1

#include <stdio.h>

int main() {
int temp;
    printf("Enter the temperature in celsius ");
    scanf("%d",&temp);
    if(temp<15){
        printf("cold");
    }
    else if(temp<30 && temp>15) {
        printf("normal");
        
    }
    else  {
        printf("hot");
    }
    return 0;
}
 # task 2
 #include <stdio.h>

int main() {
int balance;
    printf("balance ");
    scanf("%d",&balance);
    if (balance < 500){
        printf("low balance");
    }
    else if (balance>500 && balance <2000 ){
        printf("sufficient balance");
    }
    else{
        printf("premium balance");
    }
    return 0;

    # task 3 
    #include <stdio.h>

int main() {
int appointment, doctorAvailable,
 registrationComplete;
    printf("appointment ? , if yes press 1 if no press 0"  );
    scanf("%d",&appointment);
    printf("doctorAvailable ? , if yes press 1 if no press 0"  );
    scanf("%d",&doctorAvailable);
     printf("registrationCompleted ? , if yes press 1 if no press 0"  );
    scanf("%d",&registrationCompleted);

    
        if (doctorAvailable==1 && registrationCompleted==1 &&appointment==1){
        printf("you can meet doctor");
    }
    else {
        printf("you cannot meet doctor");
    }
    return 0;
}
 # task 4
#include <stdio.h>

int main() {
int restaurantOpen,itemAvailable, balanceSufficient;
    printf("restaurantOpen ? , if yes press 1 if no press 0"  );
    scanf("%d",&restaurantOpen);
    printf( "itemAvailable ? , if yes press 1 if no press 0"  );
    scanf("%d",&itemAvailable);
     printf( "balanceSufficient ? , if yes press 1 if no press 0"  );
    scanf("%d",&balanceSufficient);

    
        if (restaurantOpen==1  &&itemAvailable==1 && balanceSufficient==1){
        printf("appropriate order status.");
    }
    else {
        printf(" not appropriate order status.");
    }
    return 0;
}

# task 5

#include <stdio.h>

int main() {
int  mainchoice , sub_choices;
    printf("choose one operation 1 for Balance Inquiry, 2 for Cash Withdrawal, 3 for Cash Deposit, and 4 for PINChange.");
    scanf("%d", &mainchoice);
    switch( mainchoice){
        case 1 :
        printf( "saving accounts \n current account choice(1-2)");
    scanf("%d",&sub_choices);
    switch(sub_choices){
        case 1 : printf("operation: balance inquiry  account :saving ");
        break;
        case 2 :
        printf("operation: balance inquiry : current");
        break;
        default: printf("invalid account selection");break;
    }
        break;
    case 2 : printf( "saving accounts \n current account choice(1-2)");
    scanf("%d",&sub_choices);
          switch(sub_choices){
              case 1 : printf("cash withdrawal : saving ");break;
                  case 2 : printf("cash withdrawal : current ");break;
                      default: printf("invalid account selection");
                       break;}
        break;
              case 3 : 
                  printf( "saving accounts \n current account choice(1-2)");
                  scanf("%d", &sub_choices);
                  
          switch(sub_choices){
              case 1 : printf("Cash Deposit, : saving ");break;
                  case 2 : printf("Cash Deposit, : current ");break;
                      default: printf("invalid account selection");
                       break;
          }break;
        case 4 :
            printf("pin change");
            break;
            default: 
                printf("invalid account selection");
                       break;}
    return 0;
}
 
