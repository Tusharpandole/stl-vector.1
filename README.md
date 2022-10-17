# stl-vector.1
#include <iostream>
#include <vector>

using namespace std;

int main()
{
    vector<int>v ;
    //for inilization of all element with the same number in an array 
    vector<int>a(5,1) ;
    
    //for coping one vector in another 
    vector<int>last(a) ;
    cout << "The capacity of the vector is " <<  v.capacity() <<  endl ;
    v.push_back(5) ;
    v.push_back(6) ;
     cout << "The capacity of the vector is " <<  v.capacity() <<  endl ;
     v.push_back(7) ;
     cout << "The size of the vector is " << v.size() <<  endl ;
   cout << "The capacity of the vector is " <<  v.capacity() <<  endl ;
   cout << "The element at the index 2 is " << v.at(2) << endl ;
   cout << "The front element is " << v.front() <<  endl ;
   cout << "All the element off the array are " << endl ;
   for(int i : v) 
   {
       cout << i <<  " " <<endl;
   }
   cout << "The vector a = " << endl ;
   for(int i : a)
   {
       cout << i << " " << endl  ;
   }
   cout << "The vector named last will be "<< endl ;
   for(int i : last)
   {
       cout << i << " " ;
   }
    return 0;
}
