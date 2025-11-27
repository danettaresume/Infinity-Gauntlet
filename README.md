#include <iostream>
#include <string>

bool mindStoneChallenge() {
    std::string answer;
    std::cout << "I speak without a mouth and hear without ears. What am I?\n> ";
    std::getline(std::cin, answer);
    return (answer == "echo" || answer == "Echo");
}

int main() {
    std::cout << "Welcome, Iron Man. Lock the Mind Stone.\n";
    std::cin.ignore();
    if (mindStoneChallenge()) {
        std::cout << "✅ Mind Stone locked!\n";
    } else {
        std::cout << "❌ Wrong. Thanos is closer.\n";
    }
    return 0;
}

