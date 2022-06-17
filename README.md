# Hello-world
This is hello world repository


#include <iostream>
#include<bits/stdc++.h>
using namespace std;

int main() {
     array<int,5> arr ={1,2,3,3,5};
     array<int,2> arr2;
     unordered_map<int,int> mp;
     
       for(int i=0; i<5; i++)
           mp[arr[i]]++;
    
       for(auto itr=mp.begin(); itr!=mp.end(); itr++){
          if(itr->second>1)
            arr2[0]= itr->first;
       }
       
       int count =1;
       for(auto itr=mp.begin(); itr!=mp.end(); itr++){
          if(mp.find(count)== mp.end()){
                arr2[1]=count;
          }
          count++ ; 
       }
       
       for(int i =0; i<2; i++) cout<<arr2[i]<<" ";
       
    
     return 0;
}
