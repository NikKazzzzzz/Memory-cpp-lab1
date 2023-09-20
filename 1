#include <iostream>
#include <cstring>
#include <stdexcept> // Для std::out_of_range

using namespace std;

class String {
    char* buffer = nullptr;
    int size = 0;

public:
    String(int _size) : buffer(new char[_size]), size(_size - 1) {}

    String(const String& str) : buffer(new char[str.size + 1]), size(str.size) {
        strcpy(buffer, str.buffer);
    }

    String() : buffer(nullptr), size(0) {}

    String(const char* p) : buffer(new char[strlen(p) + 1]), size(strlen(p)) {
        strcpy(buffer, p);
    }

    ~String() {
        delete[] buffer;
    }

    char& operator[](int i) {
        if (i < 0 || i >= size) {
            throw std::out_of_range("Invalid index");
        }
        return buffer[i];
    }

    const char& operator[](int i) const {
        if (i < 0 || i >= size) {
            throw std::out_of_range("Invalid index");
        }
        return buffer[i];
    }

    String& operator=(const String& str) {
        if (this != &str) {
            if (size < str.size) {
                delete[] buffer;
                buffer = new char[str.size + 1];
            }
            strcpy(buffer, str.buffer);
            size = str.size;
        }
        return *this;
    }

    String operator+(const String& str) const {
        String sum(size + str.size + 1);
        strcpy(sum.buffer, buffer);
        strcat(sum.buffer, str.buffer);

        return sum;
    }

    String& operator+=(const String& str) {
        char* new_buffer = new char[size + str.size + 1];
        strcpy(new_buffer, buffer);
        strcat(new_buffer, str.buffer);
        delete[] buffer;
        size = size + str.size + 1;
        buffer = new_buffer;
        return *this;
    }

    bool operator==(const String& str) const {
        return strcmp(buffer, str.buffer) == 0;
    }

    bool operator!=(const String& str) const {
        return strcmp(buffer, str.buffer) != 0;
    }

    bool operator>(const String& str) const {
        return strcmp(buffer, str.buffer) > 0;
    }

    bool operator<(const String& str) const {
        return strcmp(buffer, str.buffer) < 0;
    }

    friend ostream& operator<<(ostream& out, const String& str) {
        if (str.size == 0) {
            out << "The string is empty";
        } else {
            out << "string='" << str.buffer << "' size=" << str.size;
        }
        return out;
    }
    friend istream& operator>>(istream& in, String& str) 
{
    // Удаляем старый буфер, если он существует
    delete[] str.buffer;

    int size = 100; 
    char *new_buffer = new char[size];
    int i = 0;
    char ch;

    while ((ch = getc(stdin)) != '\n') {
         if(i == size - 1) {
            
            new_buffer[i] = '\0';
            str.buffer = new_buffer;
            new_buffer = new char[size *=2];
            strcpy(new_buffer, str.buffer);
            delete[] str.buffer;
            
            
            
        }
        new_buffer[i++] = ch;
    }
    
    new_buffer[i] = '\0';
    str.buffer = new_buffer;
    str.size = i;

    return in;
}


    
};

int main() {
    String str1("Hello");
    String str2;

    cout << "Введи строку для склейки: ";
    cin >> str2;

    str1 += str2;

    cout << "Результат склейки: " << str1 << endl;

    return 0;
}
