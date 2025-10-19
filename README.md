//QUESTION FOUR PART B.

package vu.babyfeedingschedule;


public class BabyFeedingSchedule {
    //Breakdown of the problem.
    //Cup size: 0.5 litres;
    //Porridge: 2 litres, 4 halfcups, 4 feedings, 45 minutes between each feedings;
    //Milk: 2 litres, 4 full cups, 4 feedings, 30 minutes between each feedings;
    //Then Calcualation breakdown;
    //Porridge total time taken = intervals * 45 minutes;
    //Milk total time taken = intervals * 30 minutes;
             

    public static void main(String[] args) {
        //constants
                double Cupsize = 0.5;
                double PorridgeVolume = 2.0;
                double MilkVolume = 2.0;
                
        //Calcualte the number of Feedings.
        int PorridgeFeedings = (int)(PorridgeVolume / Cupsize);
        int MilkFeedings = (int)(MilkVolume / Cupsize);
        
        //Feeding intervals.
        int PorridgeInterval = 45;
        int MilkInterval = 30;
        
        //Time taken for each feedings = (number of intervals) * interval time.
        int PorridgeTime = (PorridgeFeedings - 1) * PorridgeInterval;
        int MilkTime = (MilkFeedings -1) * MilkInterval;
        
        //Total time taken = PorridgeTime + MilkTime.
        int Totaltime = PorridgeTime + MilkTime;
        
                                
        System.out.println("Total time to finish all the meals:"+ Totaltime+"minutes");
    }
}
