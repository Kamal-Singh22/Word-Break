# Word-Break
Given a string s and a dictionary of words wordDict, return true if s can be segmented into a space-separated sequence of one or more dictionary words.
Explanation:
Use Dynamic Programming (dp array) to track whether s[0:i] can be formed using words in wordDict.
Iterate through all substrings and check if it exists in the dictionary.
If dp[j] is true and s[j:i] exists in wordDict, then dp[i] = true.
Return dp[s.length()] as the final result.
Time Complexity: O(n^2), where n is the length of s.
Space Complexity: O(n), due to the dp array.
