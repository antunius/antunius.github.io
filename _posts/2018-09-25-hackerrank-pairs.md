---
layout: post
title: "Hackerrank Solution Pairs"
author: "Marcus"
---

{% highlight c++ %}
int pairs(int k, vector<int> arr) {
    int ans=0;
    sort(arr.begin(),arr.end());
    for(int i=0; i < arr.size(); i++){
        if(binary_search(arr.begin(),arr.end(),arr[i]-k)){
            ans++;
        }
    }
    return ans;
}
{% endhighlight  %}
