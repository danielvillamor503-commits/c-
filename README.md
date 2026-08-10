#include <iostream>
#include <unistd.h>
using namespace std;
int main() {
string lyrics[] = {
"can we go back to the days our love was true? ",
"can somebody tell me how to get things back, the way they used to be",
"oh God give me a reason",
"im down on bended knees"
};
int size = sizeof(lyrics) / sizeof(lyrics[0]);
for (int i = 0; i < size; i++) {
for (int j = 0; j < lyrics[i].length(); j++) {
cout << lyrics[i][j] << flush;
usleep(50000);
}
cout << endl;
usleep(500000);
}
return 0;
}             