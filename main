#include "std_lib_facilities.h"

int main()
{	
	
	vector<string>string_vals{ "zero", "one", "two", "three", "four", "five", "six", "seven", "eight", "nine"};
	vector<int>int_vals{ 0, 1, 2, 3, 4, 5, 6, 7, 8, 9 };

	cout << "Spell out a number and I will give you the digit;" << '\n';
	cout << "Or give me a digit and I will spell it out for you: ";
	string word_digit{};
	while (cin >> word_digit) {
        bool found = false;

        // Check if the input is a spelled-out number
        for (size_t i = 0; i < string_vals.size(); ++i) {
            if (word_digit == string_vals[i]) {
                cout << int_vals[i] << '\n';
                found = true;
                break;
            }
        }

        // If not found, check if the input is a digit
        if (!found) {
            for (size_t i = 0; i < int_vals.size(); ++i) {
                if (word_digit == to_string(int_vals[i])) {
                    cout << string_vals[i] << '\n';
                    found = true;
                    break;
                }
            }
		}

        if (!found) {
            cout << "Invalid input." << '\n';
        }
    }

	return 0;
}
