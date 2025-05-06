#include <iostream>
using namespace std;

class Hotel {
public:
    int room_number;
    string type;
    string availability;

    void book_a_room() {
        cout << "Enter room number: ";
        cin >> room_number;
        cout << "Select type of room: ";
        cin >> type;
        cout << "The availability of your booked room is: " << availability << endl;
    }    

    void check_out_a_room() {
        if (type == "vip") {
            cout << "The room is available" << endl;
        } else if (type == "vivip") {
            cout << "Sorry, the room is not available" << endl;
        }
    }

    void show_availability_room() {
        cout << "Room type: " << type << endl;
    }
};

int main() {
    Hotel ht;
    ht.book_a_room();
    ht.check_out_a_room();
    ht.show_availability_room();
    return 0;
}
