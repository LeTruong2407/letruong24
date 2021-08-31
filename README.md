#include <iostream>
#include <string>
#include <fstream>
#include <stdio.h>
#include <conio.h>
#include<ctime>
#include <vector>
#include "windows.h" 
using namespace std;






int main()
{
	string ngiu;
	while (true)
	{
		system("cls");
		cout << endl << endl;
		cout << "\t\tTEN EM LA GI Z ? ";
		getline(cin, ngiu);
		if (ngiu == "Tten")
		{
			cout << "\t\t---hiiamtten---" << endl << endl;


			
			while (true)
			{
				int i = 0;
				

				ifstream file;
				file.open("C:\\Users\\levan\\Downloads\\banner.txt", ios_base::in); // chèn file m vô (file dạng txt)
				string line;
				while (getline(file, line)) {
					cout << line << endl;
					Sleep(50);
				}
				file.close();
				

			}
		}
		else
		{
			cout << "\t\tSAI ROI ;((" << endl << endl;
			system("pause");
		}
	}
}
