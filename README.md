# C-language-codes-for-Stock-Market

#include <stdio.h>
int main ()
{   char comp[20];
    float P1, P2, P3, P4, P5, S1, S2, S3, S4, S5, R1, R2, R3, R4, R5, E1, E2, E3, E4, E5, PBIT1, PBIT2, PBIT3, PBIT4, PBIT5, I1, I2, I3, I4, I5;
    int Stock, n1, Co;
    float X1, X2, X3, X4, Y1, Y2, Y3, Y4, Z1, Z2, Z3, Z4;
    char nam[50], prt[20];
    float n, F_V, P_V, CAGR;
    double Z, X, Y;
    float P, F, N, A, B, FEV, EEB, CEB, SO, TP, EP;
    float T_P, En_P, E_P, G, RR, AA, S;


    printf("   WELCOME TO THE FUNDAMENTAL ANALYSIS OF STOCK MARKET\n      (Stock Market Are Subjected To Market Risks)\n");

    printf("\n\nWrite the name of the Company: ");
    scanf("%[^\n]", &comp);

    printf(" \n ENTER\n [1] For Balance Sheet Analysis\n\n [2] For Profit & Loss Analysis\n\n [3] For CAGR Calculation\n\n [4] For Finding Principal Value \n\n [5] For Finding Principal Value\n\n [6] For Targerting Share Price Using 'BENJAMIN GAHRAM MODEL'\n\n [7] For Targeting Share Price Using 'EV/EBIDTA MODEL'\n");
    scanf("%d", &n1);
    switch(n1)
    {
    case 1:

        printf("   COMPANY BALANCE SHEET ANALYSIS\n \n");

        printf("Name of Company: %s", comp);

        printf("\n   STEP:1: ''SHARE CAPITAL (in Cr.)'' ");

        printf("\n 1st year: ");
        scanf("%f", &X1);
        printf("\n 2nd year: ");
        scanf("%f", &X2);
        printf("\n 3rd year: ");
        scanf("%f", &X3);
        printf("\n CURRENT year: ");
        scanf("%f", &X4);

        printf("\n   STEP:2: ''RESERVES (in Cr.)''");

        printf("\n 1st year: ");
        scanf("%f", &Y1);
        printf("\n 2nd year: ");
        scanf("%f", &Y2);
        printf("\n 3rd year: ");
        scanf("%f", &Y3);
        printf("\n CURRENT year: ");
        scanf("%f", &Y4);

        printf("\n   STEP:2: ''DEBT (in Cr.)''");

        printf("\n 1st year: ");
        scanf("%f", &Z1);
        printf("\n 2nd year: ");
        scanf("%f", &Z2);
        printf("\n 3rd year: ");
        scanf("%f", &Z3);
        printf("\n CURRENT year: ");
        scanf("%f", &Z4);

        if(Y1<Y2 && Y2<Y3 && Y3<Y4 && Z1>Z2 && Z2>Z3 && Z3>Z4)
        {
            printf("%s COMPANY DECLARED AS GOOD BALANCE SHEET ", nam);
        }
        else {
            if(Y1>Y2 && Y2>Y3 && Y3>Y4 && Z1<Z2 && Z2<Z3 && Z3<Z4)
            {
                printf("%s   COMPANY DECLARED AS BAD OR POOR BALANCE SHEET ", comp);
            }
            else {
                printf("%s   COMPANY DECLARED AS AVERAGE AND NOT AT ALL GOOD BALANCE SHEET ", comp);
            }
        }
        break;

    case 2:

    {

        printf("      PROFIT & LOSS STATEMENT ANSLYSIS");

        printf("\n\nName of the Company: %s \n", comp);


        printf("\n  Enter Net Profits: ");
        printf("\n1st Year: ");
        scanf("%f", &P1);

        printf("\n2nd Year: ");
        scanf("%f", &P2);

        printf("\n3rd Year: ");
        scanf("%f", &P3);

        printf("\n4th Year: ");
        scanf("%f", &P4);

        printf("\n5th Year: ");
        scanf("%f", &P5);

        printf("\n  Enter Net Sales: ");
        printf("\n1st Year: ");
        scanf("%f", &S1);

        printf("\n2nd Year: ");
        scanf("%f", &S2);

        printf("\n3rd Year: ");
        scanf("%f", &S3);

        printf("\n4th Year: ");
        scanf("%f", &S4);

        printf("\n5th Year: ");
        scanf("%f", &S5);

        printf("\n  Enter The Consumption Of Raw Material: ");
        printf("\n1st Year: ");
        scanf("%f", &R1);

        printf("\n2nd Year: ");
        scanf("%f", &R2);

        printf("\n3rd Year: ");
        scanf("%f", &R3);

        printf("\n4th Year: ");
        scanf("%f", &R4);

        printf("\n5th Year: ");
        scanf("%f", &R5);

        printf("\n  Enter Employees Cost: ");
        printf("\n1st Year: ");
        scanf("%f", &E1);

        printf("\n2nd Year: ");
        scanf("%f", &E2);

        printf("\n3rd Year: ");
        scanf("%f", &E3);

        printf("\n4th Year: ");
        scanf("%f", &E4);

        printf("\n5th Year: ");
        scanf("%f", &E5);

        printf("\n  Enter PBIT: ");
        printf("\n1st Year: ");
        scanf("%f", &PBIT1);

        printf("\n2nd Year: ");
        scanf("%f", &PBIT2);

        printf("\n3rd Year: ");
        scanf("%f", &PBIT3);

        printf("\n4th Year: ");
        scanf("%f", &PBIT4);

        printf("\n5th Year: ");
        scanf("%f", &PBIT5);

        printf("\n  Enter Intrests Paid: ");
        printf("\n1st Year: ");
        scanf("%f", &I1);

        printf("\n2nd Year: ");
        scanf("%f", &I2);

        printf("\n3rd Year: ");
        scanf("%f", &I3);

        printf("\n4th Year: ");
        scanf("%f", &I4);

        printf("\n5th Year: ");
        scanf("%f", &I5);

        if(P1<P2 && P2<P3 && P3<P4 && P4<P5 && S1<S2 && S2<S3 && S3<S4 && S4<S5 && R1<R2 && R2<R3 && R4<R5 && E1<E2 && E2<E3 && E3<E4 && E4<E5 && PBIT1<PBIT2 && PBIT2<PBIT3 && PBIT3<PBIT4 && PBIT4<PBIT5 && I1>I2 && I2>I3 && I3>I4 && I4>I5)
            printf("\n      P & L Statement of %s is Very Good.", comp);
        else
        {   if(P1>P2 && P2>P3 && P3>P4 && P4>P5 && S1>S2 && S2>S3 && S3>S4 && S4>S5 && R1>R2 && R2>R3 && R4>R5 && E1>E2 && E2>E3 && E3>E4 && E4>E5 && PBIT1>PBIT2 && PBIT2>PBIT3 && PBIT3>PBIT4 && PBIT4>PBIT5 && I1<I2 && I2<I3 && I3<I4 && I4<I5)
            {
                printf("\n      P & L Statement of %s is Very Bad.", comp);
            }
            else {
                printf("\n      P & L Statement of %s is Not at all Very Good or say it is Average or Good.", comp);
            }

        }

        break;
        case 3:

            printf("   'COMPOUND ANNUAL GROWTH RETURNS (C.A.G.R) CALCULATOR'\n");
            printf("\nParticulars\n (Eg:- EPS, Net profit, Sales,etc..) of %s", comp);

            printf("\nEnter the Principal Value: ");
            scanf("%f", &P_V);

            printf("\nEnter the Final Value: ", prt);
            scanf("%f", &F_V);

            printf("\nEnter the No. of years in Span of Principal to final Value of: ");
            scanf("%f", &n);

            X=F_V/P_V;
            Y=1/n;

            Z=pow(X,Y);
            CAGR=(Z-1)*100;

            printf("\nC.A.G.R of %s in %0.2f years is %0.2f%%%.", comp, n, CAGR);

            break;
        case 4:
            printf("   'COMPOUND ANNUAL GROWTH RETURNS (C.A.G.R) CALCULATOR'\n");
            printf("\nEnter the name of Particulars\n (Eg:- EPS, Net profit, Sales,etc..) of %s ", comp);

            printf("\nEnter the Final Value: ");
            scanf("%f", &F_V);


            printf("\nEnter the No. of years in Span of Principal to final Value: ");
            scanf("%f", &n);

            printf("\nEnter the CAGR: ");
            scanf("%f", &CAGR);


            X=CAGR/100+1;
            Y=n;

            Z=pow(X,Y);
            P_V=F_V/Z;

            printf("\nPrincipal Value of %s in %0.2f years is %0.2f.", comp, n, P_V);

            break;

        case 5:

            printf("   'RETURN CALCULATOR'\n");
            printf("\nName of Particulars\n (Eg:- EPS, Net profit, Sales,etc..): %s", comp);

            printf("\nEnter the Final Value:");
            scanf("%f", &F_V);

            printf("\nEnter the No. of years in Span of Principal to final Value: ");
            scanf("%f", &n);

            printf("\nEnter the CAGR: ");
            scanf("%f", &CAGR);

            X=CAGR/100+1;
            Y=n;

            Z=pow(X,Y);
            P_V=Z*F_V;

            printf("\nFinal Value of %s in %0.2f years is %0.2f.", comp, n, P_V);

            break;
        case 6:


            printf("\n      TARGETING SHARE PRICE USING BENJAMIN GRAHAM MODEL\n");
            printf("\nName of the company: %s", comp);

            printf("\nEnter the Current Share price: ");
            scanf("%f", &S);

            printf("\nEnter the TTM EPS: ");
            scanf("%f", &E_P);

            printf("\nEnter the cureent Repo Rate of Bank: ");
            scanf("%f", &RR);

            printf("\nEnter the (AAA Rated) Indian Bond Yield: ");
            scanf("%f", &AA);

            printf("\nEnter the growth rate of E.P.S.: ");
            scanf("%f", &G);

            printf("\nEnter \n (1) If it is Average Company \n (2) If it is  large Company  ");
            scanf("%d", &Co);
            switch(Co)
            {
            case 1:
                T_P=E_P*(7+1*G)*RR/AA;
                En_P=2*T_P/3;
                printf("\nThe target price of %s is %0.2f \n AND \n", comp, T_P);
                printf("Entry price is %0.2f", En_P);

                break;
            case 2:
                T_P=E_P*(8.5+1*G)*RR/AA;
                En_P=2*T_P/3;
                printf("\nThe target price of %s is %0.2f \n AND \n", comp, T_P);
                printf("Entry price is %0.2f", En_P);
            }

            if(T_P>S)
            {
                printf("\nCurrently price of %s is Undervalued.", comp);
            }
            else {
                printf("\nCurrently price of %s is Overvalued.\n \n", comp);
            }


            return(0);
        }


    case 7:


        printf("     TARGERTING PRICE USING EV/EBDITA MODEL\n Use at least 5 years daata\n");

        printf("\nName Of The Company:%s ", comp);


        printf("\nEnter the principal Value of ebita: ");
        scanf("%f", &P);

        printf("\nEnter the final  Value of ebita: ");
        scanf("%f", &F);


        printf("\n No. of years Between Principal and final Value of ebita:  ");
        scanf("%f", &N);


        printf("\nEnter the Curent Value of EV/EBIDTA: ");
        scanf("%f", &CEB);

        printf("\nEnter the total share Outstanding: ");
        scanf("%f", &SO);

        X=F/P;
        Y=1/N;
        Z=pow(X,Y);
        CAGR=(Z-1)*100;

        A=CAGR/100;
        B=A+1;
        EEB=B*F;

        FEV=CEB*EEB;

        TP=FEV/SO;
        EP=TP*2/3;

        printf("\nTarget Price of %s is Rs.%0.2f and \nEntry price is  Rs.%0.2f", comp, TP, EP);

    default:
        printf("!!INVALID CHOICE!!!");
        break;
    }

    return(0);
}
