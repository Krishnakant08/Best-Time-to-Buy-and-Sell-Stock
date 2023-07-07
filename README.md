class Solution {
public:
    int maxProfit(vector<int>& prices) {

    
         int ans=0;
         int min=prices[0];
         int n=prices.size();
         for(int i=1;i<n;i++){
              if(prices[i]<=min){
                  min=prices[i];
              }
              ans=max(ans,prices[i]-min);
               }
         
         return ans;
    } 
};
