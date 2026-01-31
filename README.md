# CodeAlpha_CGPA-calculator
#include <iostream>
using namespace std;

int main() {
    int n;
    cout << "Enter number of courses: ";
    cin >> n;

    float grade, totalGradePoints = 0;
    int credits, totalCredits = 0;

    for (int i = 1; i <= n; i++) {
        cout << "\nCourse " << i << endl;
        cout << "Enter grade point: ";
        cin >> grade;
        cout << "Enter credit hours: ";
        cin >> credits;

        totalGradePoints += grade * credits;
        totalCredits += credits;
    }

    float gpa = totalGradePoints / totalCredits;

    cout << "\nTotal Credits: " << totalCredits << endl;
    cout << "GPA: " << gpa << endl;
    cout << "CGPA: " << gpa << endl;

    return 0;
}
