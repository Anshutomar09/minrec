# minrec

class Solution {
public:
    vector<int> constructRectangle(int area) {
        vector<int> ans;
        int b=1;

        for(int i=1;i<=sqrt(area);i++){
            if(area%i==0){
             b=i;
            }
            
        }
        ans.push_back(area/b);
        ans.push_back(b);
        return ans;
    }
};
