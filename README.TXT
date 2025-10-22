
Answers to lab 7, part I:

Part I:

#1 10am (227), 2pm (227), 6pm(237).

#2 private Person[] people;

#3 private boolean[] vacant;

#4 Used in every method except printData(). 

#5 int[] counts;
   boolean[true(or false)] occupied;
   
#6 a) double[60] readings;
   b) String[90] urls;
   c) TicketMachine[5] machines;

#7 1 object, String array with 20 slots. No actual string object created.

#8 double[] prices = new double[50];

#9 Java has an error that says out of bounds refering the bounds of the array that is 24 but non-inclusive.

#10 int hour = 0;
    while(hour < hourCounts.length){
        System.out.println(hour + ": " + hourCounts[hour]);
        hour++;
    }

#11 /** * Print all the values in the marks array that are greater than mean.
    * @param marks An array of mark values.
    * @param mean The mean (average) mark. */
    public void printGreater(double[] marks, double mean) {
        for(index = 0; index < marks.length; index++) {
            if(marks[index] > mean) {
                System.out.println(marks[index]);
            }
        }
    }

#13 /** 
    * Return the number of accesses recorded in the log file. 
    */
    public int numberOfAccesses() {
        int total = 0;
        for(index = 0; index < hourCounts.length; index++){
            total += hourCounts[index];
        }
        return total;
    }

#15 for loop is better because as we iterate through the whole array we need to keep track of the hour we are at (count).

#16 In this case the issue can be fixed by making the quietestHourCount = to hourCounts[busiestHour()], this makes
    it so that the quietest hour count will be put to the highest and as it goes down the list the loop
    will find the smallest count starting from the busiest. I think this is the 
    safest method of doing so because it ensures no errors by starting from the busiestHourCount. 


