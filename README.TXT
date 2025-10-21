
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

#7 1 object, String array with 20 slots.

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

#
