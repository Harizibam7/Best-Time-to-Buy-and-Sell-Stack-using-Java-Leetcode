# Best-Time-to-Buy-and-Sell-Stack-using-Java-Leetcode
    
    class Solution {
        public int maxProfit(int[] prices) {
            int max_profit =0;
            int min_profit =prices[0];
            for(int i =0; i<prices.length;i++){
                if(prices[i]<min_profit){
                    min_profit = prices[i];
                }
                if(prices[i]-min_profit > max_profit ){
                    max_profit = prices[i]-min_profit;
                }
            }
            return max_profit;
    
        }
    }
