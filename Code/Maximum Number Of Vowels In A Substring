class Solution {
public:
    int maxVowels(string s, int k) {
        set<char> vowel({'a', 'e', 'i', 'o', 'u'});
 
        int ans = 0;
        int l = 0, r = 0;
        while(r < k) ans += vowel.count(s[r++]);
         
        int current = ans;
        while(r < s.length()){
            current += vowel.count(s[r++]);
            current -= vowel.count(s[l++]);
            ans = max(ans, current);
        }
 
        return ans;
    }
};
