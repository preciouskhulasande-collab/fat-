#include <iostream>
using namespace std;

int main() {
	int temp1, temp2, temp3;

	//Get the first temperature reading
	cout << "Enter first temperature reading: ";
	cin >> temp1;

	//Get second temperature reading
	cout << "Enter second temperature reading: ";
	cin >> temp2;

	//Check temperature increase
	if (temp2 - temp1 > 50) {
		cout << "Reduce the fryer heat before the third reading" << endl;
		return 1;
	}
	else if (temp2 - temp1 < 10) {
		cout << "Increase the heat before taking the third reading" << endl;
		return 1; 
	}

	//Get third temperature reading
	cout << "Enter third temperature reading: ";
	cin >> temp3;

	//Check if oil is ready for frying 
	if (temp3 >= 150 && temp3 <= 190) {
		cout << "You may start frying the Magwinyas" << endl;
	}
	else {
		cout << "Oil is not ready for frying" << endl;
	}
	return 0;
}
fatties 234
