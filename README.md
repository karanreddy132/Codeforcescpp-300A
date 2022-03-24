# Codeforcescpp-300A
#include <bits/stdc++.h>
using namespace std;

int main() {
	int n,a[101];
  cin >> n;
  for(int i=0;i<n;i++){
    cin >> a[i];
  }
  sort(a,a+n);
  cout << 1 << " " << a[0] << endl;
  if(a[n-1]!=0){
    cout << 1 << " " << a[n-1] << endl;
    cout << n-2 << " ";
    for(int i=1;i<n-1;i++){
      cout << a[i] << " ";
    }
  }
  else{
    cout << 2 << " " << a[n-2] << " " << a[n-3] << endl;
    cout << n-3 << " ";
    for(int i=1;i<n-3;i++){
      cout << a[i] << " ";
    }
    cout << 0;
  }
	return 0;
}
