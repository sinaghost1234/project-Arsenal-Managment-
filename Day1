// # project-Arsenal-Managment-
// 30 Days of my coding to complete this project  : Trying to defeat Final Boss from Ohio LMAO **  DAY1 **
#include <stdio.h>
#include <stdlib.h>
#include <windows.h>
#include <conio.h>

int main()
{
   // system("start sina101.mp3") ;

    page1 :  printf("** Welcome to SAM( Sina's Arsenal management ) ** \t \t \t \t \t \t \t \t  Music Played : Fit girl :) \n ") ;

    printf("1.SignUp !\n ") ;

    printf("2.Login\n ") ;

    printf("3.Exit\n ") ;

    printf(">> Please enter your choice: ") ;

    int Enterchoice ;

    char BackToFirstPage [32] ;

    scanf("%d" , &Enterchoice) ;

    if ( Enterchoice == 3 )
    {
        exit(0) ;
    }
    else if ( Enterchoice == 1 )
    {
        system("cls") ;

        printf(" SIGN UP \n \n") ;

        printf("Create your SAM Account\n \n") ;

        printf("Back to first page >> ""press 1"": \n") ;

        printf("Continue >> ""press 2"":") ;

    for ( ; ; )
      {
        gets(BackToFirstPage) ;

        if ((BackToFirstPage[0] == '1' ) && ( strlen(BackToFirstPage) == 1 ) )
        {
            system("cls") ;

            goto page1 ;
        }

           else if (BackToFirstPage[0] == '2'&& ( strlen(BackToFirstPage) == 1 ) )
        {
               break ;
        }

        else if ( strlen(BackToFirstPage) != 1 )
        {
            printf("\nEnter the correct order : ") ;
        }
       }

    struct Members
    {
        char Name_newmember[32] ;

        char LastName_newmemeber[32] ;

        char controlname[32] ;

        char id[32] ;

        char phone_Number[32] ;

        char email_Newmemeber[32] ;

        char password_Newmember [32] ;

        char password_Newmemberaccept [32] ;
    } ;

    struct Members Member ;

    FILE *ListMemberFp ;

    ListMemberFp = fopen("E:\\ListMemberFp.txt", "a+") ;

        printf("First name :");

        int i ;

        for ( i = 0 ; i <= 31 ; i++ )
        {
            Member.Name_newmember[i] = ' ';
        }

        gets(Member.Name_newmember) ;

        printf("\n") ;

        printf("Last name :");

        for ( i = 0 ; i <= 31 ; i++ )
        {
            Member.LastName_newmemeber[i] = ' ';
        }

        gets(Member.LastName_newmemeber) ;

        printf("\n") ;

        printf("Username :");

        for ( i = 0 ; i <= 31 ; i++ )
        {
            Member.controlname[i] = ' ';
        }
        gets(Member.controlname) ;

        printf("\n") ;

        printf("ID :") ;

        for ( i = 0 ; i <= 31 ; i++ )
        {
            Member.id[i] = ' ';
        }

        gets(Member.id) ;

        printf("\n") ;

        printf("Email *( Please enter the form Username@gmail/yahoo.com )* :") ;

        for ( i = 0 ; i <= 31 ; i++ )
        {
            Member.email_Newmemeber[i] = ' ';
        }

        gets(Member.email_Newmemeber) ;

        printf("\n") ;

        printf("Phone number :") ;

        for ( i = 0 ; i <= 31 ; i++ )
        {
            Member.phone_Number[i] = ' ';
        }

        gets(Member.phone_Number) ;

        printf("\n") ;

        printf("Password ( Use 8 or more characters (max is 32) with mix of letters, numbers & symbols ) :  ") ;

        int i = 0 , length_Password , safety_Password , p = 0 ;

        pw :   while ( (Member.password_Newmember[p - 1 ]!= '\r')   )
                {
                        Member.password_Newmember[p] = getch();

                    if ( (Member.password_Newmember[p - 1 ]!= '\r')  )
                        {
                            printf("*") ;
                        }

                            p++ ;
                }

                Member.password_Newmember[p-1] = '\0' ;

            for ( i = 0 ; i < length_Password ; i++ )
                {
                    if ( ( (Member.password_Newmember[i] > 64 && Member.password_Newmember[i] < 91) || (Member.password_Newmember[i] > 96 && Member.password_Newmember[i] < 123 )   ) ||( (Member.password_Newmember[i] >= 33 ) || ( Member.password_Newmember[i] <= 47 ) )|| ( (Member.password_Newmember[i] >= 58 ) || (Member.password_Newmember[i] <= 64 ) ) || ( (Member.password_Newmember[i] >= 91 ) || ( Member.password_Newmember[i] <= 96) )|| ((Member.password_Newmember[i] >= 123 ) || (Member.password_Newmember[i] <= 126) ))
                    {
                        safety_Password ++ ;
                    }

                }

            if ( safety_Password < 3 )
                {
                    printf("Use more letters and symbols for you password : like 3#ij78_43 ") ;

                    goto pw ;
                }


            else if ( (length_Password < 8) && (safety_Password > 3))
                {
                    printf(" \n Your password doesn't have enough character , ADD more and try again : ") ;

                    goto pw ;
                }

            else if ( length_Password > 8 && safety_Password > 3 )
                {
                    printf("\nYou made a strong password") ;
                    
                }
            printf("\nConfirm your password : ") ;

        pwc :while ( (Member.password_Newmemberaccept[p - 1 ]!= '\r')   )
                {
                        Member.password_Newmemberaccept[p] = getch();

                    if ( (Member.password_Newmemberaccept[p - 1 ]!= '\r')  )
                        {
                            printf("*") ;
                        }
                        p++ ;
                }

                Member.password_Newmemberaccept[p-1] = '\0' ;

            for ( i = 0 ; i <= (length_Password - 1) ; i++)
            {
                if ( Member.password_Newmemberaccept[i] != Member.password_Newmember[i])
                {
                    printf("\nConfirm your password again") ;

                    goto pwc ;
                }
            }

            fwrite(&Member , sizeof (struct Members ) , 1 , ListMemberFp) ;

            printf("\nYour account has been saved") ;
    }







}

