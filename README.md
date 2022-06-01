# fibonacci1
class Solution {
  public:
    long long int nthFibonacci(long long int n){
        //base case
        if(n == 0) 
        return 0;
        if(n == 1)
        return 1;
        //recursive call
        long long int recCall1 = nthFibonacci(n-1); 
        long long int recCall2 = nthFibonacci(n-2); // leap of faith
        //small Calculation
        long long int smallCal = recCall1  + recCall2;
        return smallCal;
    }
};
