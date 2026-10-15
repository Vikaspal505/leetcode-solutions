class Solution {
    public int sumCounts(List<Integer> nums) {
        int totalSum = 0;
        int n = nums.size();
        for (int startIndex = 0; startIndex < n; ++startIndex) {
            int[] frequency = new int[101];
            int distinctCount = 0;
            for (int endIndex = startIndex; endIndex < n; ++endIndex) {
                int currentElement = nums.get(endIndex);
                frequency[currentElement]++;
                if (frequency[currentElement] == 1) {
                    distinctCount++;
                }
                totalSum += distinctCount * distinctCount;
            }
        }
      
        return totalSum;
    }
}
