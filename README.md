# Kurs-Cpp#include<iostream>
#include<string>

using namespace std;

int main()
{
    cout << "Long Double: " << sizeof(long double) << endl;
    cout << "Double: " << sizeof(double) << endl;
    cout << "Float: " << sizeof(float) << endl;
    cout << "Long Long: " << sizeof(long long) << endl;
    cout << "Long: " << sizeof(long) << endl;
    cout << "Int: " << sizeof(int) << endl;
    cout << "Short: " << sizeof(short) << endl;
    cout << "Char: " << sizeof(char) << endl;
    cout << "Bool: " << sizeof(bool) << endl;
    cout << "String: " << sizeof(string) << endl;
    return 0;
}

#include <iostream>

using namespace std;

int main()
{

	int pierwsza_liczba, druga_liczba, trzecia_liczba;

	cout << "podaj pierwsza liczbe: ";
	cin >> pierwsza_liczba;
	cout << "podaj deuga liczbe: ";
	cin >> druga_liczba;
	cout << "podaj trzecia liczbe: ";
	cin >> trzecia_liczba; 
	cout << "średnia: " << (pierwsza_liczba + druga_liczba + trzecia_liczba) /3;

	return 0;
} 


#include <iostream>

using namespace std;

int main()
{

	int promien;

	cout << "podaj promien: ";
	cin >> promien;
	cout << "pole: " << (promien * promien * 3.14);
	cout << "obwud: " << (2 * promien * 3.14);
	return 0;
}

#include <iostream>

using namespace std;

int main()
{

	int temperatura;

	cout << "podaj temperature: ";
	cin >> temperatura;
	cout << "temperatura w fahrenheitach: " << ((temperatura * 9 / 5) + 32);

	return 0;
}

#include <iostream>

using namespace std;

int main()
{

	int benzyna, przejazd;

#include <iostream>

	using namespace std;

	cout << "podaj cene benzyny: ";
	cin >> benzyna;
		cout << " koszt przejazdu: " << (benzyna * 9 * 3.35);

		return 0;
}

#include <iostream>

using namespace std;

int main()
{

	int liczba;
	cout << "podaj liczbe całkowitą";
	cin >> liczba;
	if (liczba >= 0) {
		cout << "liczba dodatnia" << endl;
	}
	else if (liczba < 0) {
		cout << "liczba ujemna" << endl;
	}
	return 0;

}

#include <iostream>

using namespace std;

int main()
{

	int liczba;
	cout << "podaj liczbe całkowito";
	cin >> liczba;
	if (liczba < 0) {
		cout << "liczba ujemna" << endl;
	}
	else if (liczba > 0) {
		cout << "liczba dodatnia" << endl;
	}
	else if (liczba == 0) {
		cout << "zero" << endl;
	}
	return 0;
}

#include <iostream>

using namespace std;

int main()
{

	for (int liczba = 0; liczba <= 10; ++liczba) {
		cout << liczba << endl;
	}
	return 0;
}


#include <iostream>

using namespace std;

int main() {
    long long n;
    cout << "Podaj n (liczba calkowita >= 0): ";
    if (!(cin >> n)) {
        cerr << "Bledne dane wejsciowe.\n";
        return 1;
    }

    if (n < 0) {
        cerr << "Silnia jest zdefiniowana dla n >= 0.\n";
        return 1;
    }

    // unsigned long long pomieści silnie do około 20! (20! = 2_432_902_008_176_640_000)
    unsigned long long result = 1;
    for (long long i = 1; i <= n; ++i) {
        result *= static_cast<unsigned long long>(i);
    }

    cout << n << "! = " << result << '\n';
    return 0;
}

#include <iostream>

using namespace std;

#include <iostream>
#include <limits>

int main() {
    long long n;
    cout << "Podaj n (liczba calkowita >= 0): ";
    if (!(cin >> n)) {
        cerr << "Bledne dane wejsciowe.\n";
        return 1;
    }

    if (n < 0) {
        cerr << "Silnia jest zdefiniowana dla n >= 0.\n";
        return 1;
    }

    // unsigned long long pomieści silnie do około 20! (20! = 2_432_902_008_176_640_000)
    unsigned long long result = 1;
    for (long long i = 1; i <= n; ++i) {
        result *= static_cast<unsigned long long>(i);
    }

    cout << n << "! = " << result << '\n';
    return 0;
}


#include <iostream>

using namespace std;

int main() {
    long long n;
    cout << "Podaj n (liczba calkowita >= 0): ";
    if (!(cin >> n)) {
        cerr << "Bledne dane wejsciowe.\n";
        return 1;
    }

    if (n < 0) {
        cerr << "Silnia jest zdefiniowana dla n >= 0.\n";
        return 1;
    }

    // unsigned long long pomieści silnie do około 20! (20! = 2_432_902_008_176_640_000)
    unsigned long long result = 1;
    for (long long i = 1; i <= n; ++i) {
        result *= static_cast<unsigned long long>(i);
    }

    cout << n << "! = " << result << '\n';
    return 0;
}

#include <iostream>
#include <limits>

int main() {
    long long n;
    std::cout << "Podaj liczbę, dla której chcesz wypisać tabliczkę mnożenia: ";
    if (!(std::cin >> n)) {
        std::cerr << "Błędne dane wejściowe.\n";
        return 1;
    }

    int max_mul = 10; // domyślnie mnożymy od 1 do 10
    std::cout << "Do jakiego mnożnika (domyślnie 10)? ";
    if (!(std::cin >> max_mul)) {
        // jeśli użytkownik podał coś niepoprawnego, ustawiamy domyślną wartość i czyścimy strumień
        std::cin.clear();
        std::cin.ignore(std::numeric_limits<std::streamsize>::max(), '\n');
        max_mul = 10;
    }

    if (max_mul <= 0) {
        std::cerr << "Mnożnik musi być liczbą naturalną większą od 0.\n";
        return 1;
    }

    std::cout << "\nTabliczka mnożenia dla liczby " << n << " (1.." << max_mul << "):\n";
    for (int i = 1; i <= max_mul; ++i) {
        long long product = n * i;
        std::cout << n << " x " << i << " = " << product << '\n';
    }

    return 0;
}

#include <iostream>

using namespace std;

int main()
{
	int liczba;
	cout << "podaj liczbe całkowitą";
	cin >> liczba;
	if (liczba > 0) {
		cout << "liczba dodatnia" << endl;
	}
	else if (liczba < 0) {
		cout << "liczba ujemna" << endl;
	}
	else if (liczba == 0) {
		cout << "zero" << endl;
	}
	return 0;
}
