#include <algorithm>
#include <vector>
#include "inout.h"

int main() {
std::vector<int> vec;
read(vec);
std::sort(vec.begin(), vec.end());
print(vec);
return 0;
}


#ifndef INOUT_H
#define INOUT_H

#include <vector>
void print(const std::vector<int>& vec);
void read(std::vector<int>& vec);

#endif // INOUT_H


#include "inout.h"
#include <iostream>

void print(const std::vector<int>& vec) {
for (auto& elem : vec) {
std::cout << elem << std::endl;
}
}


#include "inout.h"
#include <iostream>
using namespace std;

void read(std::vector<int>& vec) {
int n;
std::cin >> n;
for (int i = 0; i < n; i++) {
int x;
std::cin >> x;
vec.push_back(x);
}
}
