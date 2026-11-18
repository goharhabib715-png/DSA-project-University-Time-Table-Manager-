
#include <iostream>
#include "Timetable.h"

using namespace std;

// University Time Management System
// Phase 1: Weekly Timetable Management

// Display timetable for a specific day
void Timetable::displayDay(int day) const {

    if (day < 0 || day >= NUM_DAYS) {
        cout << "Invalid day.\n";
        return;
    }

    cout << "\n=== " << DAY_NAMES[day] << " ===\n";

    bool found = false;
    Node* cur = head;

    while (cur != NULL) {

        if (cur->data.day == day) {

            if (!found) {
                printTableHeader();
                found = true;
            }

            printRecordRow(cur->data);
        }

        cur = cur->next;
    }

    if (!found) {
        cout << "(No classes scheduled)\n";
    }
}

// Display the complete weekly university timetable
void Timetable::displayWeek() const {

    cout << "\n====================================\n";
    cout << "   UNIVERSITY TIME MANAGEMENT SYSTEM\n";
    cout << "        WEEKLY CLASS TIMETABLE\n";
    cout << "====================================\n";

    for (int day = 0; day < NUM_DAYS; day++) {
        displayDay(day);
    }
}

// Search timetable using course code
void Timetable::searchByCourseCode(const string& code) const {

    bool found = false;

    for (Node* cur = head; cur != NULL; cur = cur->next) {

        if (cur->data.courseCode == code) {

            if (!found) {
                printTableHeader();
                found = true;
            }

            printRecordRow(cur->data);
        }
    }

    if (!found) {
        cout << "No matching course found.\n";
    }
}

// Search timetable using teacher name
void Timetable::searchByTeacher(const string& teacher) const {

    bool found = false;

    for (Node* cur = head; cur != NULL; cur = cur->next) {

        if (cur->data.teacher == teacher) {

            if (!found) {
                printTableHeader();
                found = true;
            }

            printRecordRow(cur->data);
        }
    }

    if (!found) {
        cout << "No matching teacher found.\n";
    }
}

// Search timetable using classroom number
void Timetable::searchByRoom(const string& room) const {

    bool found = false;

    for (Node* cur = head; cur != NULL; cur = cur->next) {

        if (cur->data.room == room) {

            if (!found) {
                printTableHeader();
                found = true;
            }

            printRecordRow(cur->data);
        }
    }

    if (!found) {
        cout << "No matching classroom found.\n";
    }
}

// Search timetable using section name
void Timetable::searchBySection(const string& section) const {

    bool found = false;

    for (Node* cur = head; cur != NULL; cur = cur->next) {

        if (cur->data.section == section) {

            if (!found) {
                printTableHeader();
                found = true;
            }

            printRecordRow(cur->data);
        }
    }

    if (!found) {
        cout << "No matching section found.\n";
    }
}

