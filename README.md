#include <bits/stdc++.h>
#define ll long long int

using namespace std;

int main() {
	ll n;
	cin>>n;
	map<ll,ll> m;
	
	for(ll i=0;i<n;i++){
		
		ll gh;
		cin>>gh;
		m[gh*1000000+i]=gh;
		
		
	}
	ll x=0;
	map<ll,ll>::iterator it;
	ll k=1;
	for(it=m.begin();it!=m.end();it++){
		x+=abs((*it).second-k);
		k++;
	}
	
	cout<<x<<endl;
	return 0;
}
