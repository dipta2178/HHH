# HHH
#include &lt;iostream> #include "binarysearchtree.cpp"  using namespace std;  int main() {     int n;     TreeType&lt;int> t;     if( t.IsEmpty())         cout&lt;&lt;"Tree Is Empty "&lt;&lt;endl;     else         cout&lt;&lt;"Tree Is Not Empty "&lt;&lt;endl;     cout&lt;&lt;"Insert 10 item: "&lt;&lt;endl;     for(int i = 0; i&lt;10; i++)     {         cin>>n;         t.InsertItem(n);     }     if( t.IsEmpty())         cout&lt;&lt;"Tree Is Empty "&lt;&lt;endl;     else         cout&lt;&lt;"Tree Is Not Empty "&lt;&lt;endl;     int l = t.LengthIs();     cout&lt;&lt;"length is: "&lt;&lt;l&lt;&lt;endl;     cout&lt;&lt;"Enter a number for search"&lt;&lt;endl;     bool found  = false;     cin>>n;     t.RetrieveItem(n,found);     if(found == true)         cout&lt;&lt;"Item is found"&lt;&lt;endl;     else         cout&lt;&lt;"Item is not found"&lt;&lt;endl;         cout&lt;&lt;"Enter a number for search"&lt;&lt;endl;      cin>>n;     t.RetrieveItem(n,found);     if(found == true)         cout&lt;&lt;"Item is found"&lt;&lt;endl;     else         cout&lt;&lt;"Item is not found"&lt;&lt;endl;      cout&lt;&lt;endl&lt;&lt;"List in In Order: ";     t.PrintInOrder(IN_ORDER);     cout&lt;&lt;endl&lt;&lt;"List in Pre Order: ";     t.PrintInOrder(PRE_ORDER);     cout&lt;&lt;endl&lt;&lt;"List in Post Order: ";     t.PrintInOrder(POST_ORDER);      return 0; }
