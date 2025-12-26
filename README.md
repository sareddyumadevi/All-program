class A
{
    public static void main(String[] args)
    {
        int[] ticket={52,94,24,62,65,14,25,37,53};
        int[] player1={39,85,26,45,75,15,35,65,95,25};
        int[] player2={65,28,19,46,73,13,93,87,33,44};
        
        int count1=0;
        int count2=0;
        
                for(int i=0;i<ticket.length;i++)
               {
                for(int j=0;j<player1.length;j++)
                {
                    if(ticket[i]==player1[j])
                    {
                         count1++; 
                    }
                }
                for(int k=0;k<player2.length;k++)
                {
                    if(ticket[i]==player2[k])
                    {
                         count2++; 
                    }
                }
               
            
        }
        if (count1 > count2) {
            System.out.println("Player 1 is the winner!");
        } else if (count1 < count2) {
            System.out.println("Player 2 is the winner!");
        } else {
            System.out.println("It's a tie!");
        }
    }
}
