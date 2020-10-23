#include <iostream>
int inputs[5];
int length = sizeof(inputs)/sizeof(inputs[0]);
int main() {
  for(int i = 0; i<length; i++){
    int x;
    std::cout << "Enter " + std::to_string(5-i) + " more numbers.";
    std::cin >> x;
    inputs[i]=x;
  }
  int results = 0;
  for(int i = 0; i<length; i++){
    if(inputs[i]%2==0){
      results += inputs[i];
    }
  }
  std::cout << "Sum of even numbers = " + std::to_string(results);
}