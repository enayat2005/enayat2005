
- 👋 Hi, I’m @enayat2005
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
enayat2005/enayat2005 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
include <iostream>
using namespace std;

bool isPrime(int n) {
    if (n <= 1) return false;
    for (int i = 2; i*i <= n; ++i) {
        if (n % i == 0) return false;
    }
    return true;
}

int main() {
    int num;
    cout << "Enter a number: ";
    cin >> num;

    if (isPrime(num))
        cout << num << " is a prime number.";
    else
        cout << num << " is not a prime number.";
}
🟦 2. Reverse a String
cpp
Copy
Edit
#include <iostream>
#include <string>
using namespace std;

int main() {
    string str;
    cout << "Enter a string: ";
    cin >> str;

    for (int i = str.length() - 1; i >= 0; i--)
        cout << str[i];
}
🟦 3. Factorial of a Number
cpp
Copy
Edit
#include <iostream>
using namespace std;

int main() {
    int n;
    unsigned long long factorial = 1;

    cout << "Enter a positive integer: ";
    cin >> n;

    for(int i = 1; i <= n; ++i) {
        factorial *= i;
    }

    cout << "Factorial of " << n << " = " << factorial;
}
🟦 4. Fibonacci Series (Iterative)
cpp
Copy
Edit
#include <iostream>
using namespace std;

int main() {
    int n, t1 = 0, t2 = 1, nextTerm;
    cout << "Enter the number of terms: ";
    cin >> n;

    cout << "Fibonacci Series: ";

    for (int i = 1; i <= n; ++i) {
        cout << t1 << " ";
        nextTerm = t1 + t2;
        t1 = t2;
        t2 = nextTerm;
    }
}
🟦 5. Check for Palindrome Number
cpp
Copy
Edit
#include <iostream>
using namespace std;

int main() {
    int n, reversed = 0, original, remainder;
    cout << "Enter an integer: ";
    cin >> n;
    original = n;

    while (n != 0) {
(int i= 1 ; <=n;++i
cout <<  t1 '''';
nextterm = t1 + t2;
import java.util.Scanner;

public class EvenOdd {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int num = sc.nextInt();

        if (num % 2 == 0)
            System.out.println(num + " is even.");
        else
piblic class evanodd
public statics viod main string {} arags)
        scanner sc = new scanner syestem(syestem .in);
        int num print.(enter(syestem.in);
        int num= sc.nextint();
ction Sci-Fi', 'Action Crime Thriller', 'Action Sci-Fi Adventure',
            'Action Sci-Fi', 'Action Crime Drama', 'Action Sci-Fi Thriller',
            'Adventure Drama Sci-Fi', 'Action Crime Drama', 'Crime Drama Thriller', 'Action Adventure'
        ]
    }
    return pd.DataFrame(data)

# Step 2: Vectorize genre using TF-IDF
def vectorize_genres(df):
    tfidf = TfidfVectorizer(stop_words='english')
    tfidf_matrix = tfidf.fit_transform(df['genre'])
    return tfidf_matrix

# Step 3: Compute similarity matrix
def compute_similarity(tfidf_matrix):
    return cosine_similarity(tfidf_matrix, tfidf_matrix)

# Step 4: Recommend movies
def recommend_movies(title, df, similarity_matrix, top_n=5):
    if title not in df['title'].values:
        return f"Movie '{title}' not found in database."

    idx = df[df['title'] == title].index[0]
    similarity_scores = list(enumerate(similarity_matrix[idx]))
    similarity_scores = sorted(similarity_scores, key=lambda x: x[1], reverse=True)
    top_indices = [i[0] for i in similarity_scores[1:top_n+1]]
    
    recommended_titles = df['title'].iloc[top_indices].tolist()
    return recommended_titles

# Main Execution
if __name__ == "__main__":
    df = load_data()
    tfidf_matrix = vectorize_genres(df)
    similarity_matrix = compute_similarity(tfidf_matrix)

    movie_to_search = "The Matrix"
    recommendations = recommend_movies(movie_to_search, df, similarity_matrix)

if title not in df{title} 
trfif matrix = vectory genres (df)
recomend titals =df [yitle] int{ffg(hghj) uh2hrh
DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Enayat's Portfolio</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f7f9fc;
      margin: 0;
      padding: 0;
      text-align: center;
    }

    header {
      background-color: #4a90e2;
      color: white;
      padding: 30px 0;
    }

    section {
      padding: 20px;
    }

    .btn {
      background-color: #4a90e2;
      color: white;
      border: none;
      padding: 10px 20px;
      font-size: 16px;
      cursor: pointer;
      border-radius: 5px;
      margin-top: 10px;
    }

    footer {
      background: #222;
      color: white;
      padding: 10px;
      position: fixed;
      width: 100%;
      bottom: 0;
    }
  </style>
</head>
<body>

  <header>
    <h1>Hello, I'm Enayat</h1>
    <p>B.Tech Student | Future Engineer | Movie Lover</p>
  </header>

  <section>
    <h2>About Me</h2>
    <p>I am a dedicated engineering student from Nalanda, passionate about technology, music, and spending time with family.</p>
  </section>

  <section>
    <h2>Contact</h2>
    <p>Email: enayat@example.com</p>
    <button class="btn" onclick="alert('Thanks for clicking! I will reach out soon.')">Say Hello</button>
  </section>

  <helder<p>  
#include <iostream>
#include <fstream>
#include <iomanip>
using namespace std;

class Account {
private:
    int accountNumber;
    string name;
    double balance;

public:
    void createAccount() {
        cout << "\nEnter Account Number: ";
        cin >> accountNumber;
        cout << "Enter Account Holder Name: ";
        cin.ignore();
        getline(cin, name);
        cout << "Enter Initial Deposit: ";
        cin >> balance;
        cout << "\nAccount Created Successfully!\n";
    }

    void showAccount() const {
        cout << "\nAccount Number: " << accountNumber;
        cout << "\nHolder Name: " << name;
        cout << "\nBalance: ₹" << fixed << setprecision(2) << balance << endl;
    }

    void deposit(double amount) {
        balance += amount;
    }

    void withdraw(double amount) {
        if (amount > balance) {
            cout << "Insufficient balance!\n";
        } else {
            balance -= amount;
        }
    }

    int getAccountNumber() const {
        return accountNumber;
    }

    double getBalance() const {
        return balance;
    }

    void report() const {
        cout << left << setw(12) << accountNumber
             << setw(20) << name
             << "₹" << fixed << setprecision(2) << balance << endl;
    }

    void modify() {
        cout << "\nModify Account Holder Name: ";
        cin.ignore();
        getline(cin, name);
        cout << "Modify Balance: ";
        cin >> balance;
        cout << "Account Updated!\n";
    }
};

// Function Prototypes
void writeAccount();
void displayAccount(int);
void depositWithdraw(int, int); // 1 for deposit, 2 for withdraw
void displayAll();
void modifyAccount(int);
void deleteAccount(int);

// Main Function
int main() {
    int choice;
    int accNo;

    do {
        cout << "\n===== BANK MENU =====\n";
        cout << "1. New Account\n";
        cout << "2. Display Account\n";
        cout << "3. Deposit Amount\n";
        cout << "4. Withdraw Amount\n";
        cout << "5. All Accounts\n";
        cout << "6. Modify Account\n";
        cout << "7. Delete Account\n";
        cout << "0. Exit\n";
        cout << "Enter Your Choice: ";
        cin >> choice;

        switch (choice) {
        case 1:
            writeAccount();
            break;
        case 2:
            cout << "Enter Account Number: ";
            cin >> accNo;
            displayAccount(accNo);
            break;
        case 3:
            cout << "Enter Account Number: ";
            cin >> accNo;
            depositWithdraw(accNo, 1);
            break;
        case 4:
            cout << "Enter Account Number: ";
            cin >> accNo;
            depositWithdraw(accNo, 2);
            break;
        case 5:
            displayAll();
            break;
        case 6:
            cout << "Enter Account Number: ";
            cin >> accNo;
            modifyAccount(accNo);
            break;
        case 7:
            cout << "Enter Account Number: ";
            cin >> accNo;
            deleteAccount(accNo);
            break;
        case 0:
            cout << "Thanks for using Bank System. Goodbye!\n";
            break;
        default:
            cout << "Invalid choice. Try again.\n";
        }
    } while (choice != 0);

    return 0;
}

// Function Definitions

void writeAccount() {
    Account acc;
    ofstream outFile("accounts.dat", ios::binary | ios::app);
    acc.createAccount();
    outFile.write(reinterpret_cast<char *>(&acc), sizeof(Account));
    outFile.close();
}

void displayAccount(int n) {
    Account acc;
    ifstream inFile("accounts.dat", ios::binary);
    bool found = false;
    while (inFile.read(reinterpret_cast<char *>(&acc), sizeof(Account))) {
        if (acc.getAccountNumber() == n) {
            acc.showAccount();
            found = true;
            break;
        }
    }
    inFile.close();
    if (!found)
        cout << "\nAccount Not Found!\n";
}

void depositWithdraw(int n, int option) {
    Account acc;
    fstream file("accounts.dat", ios::binary | ios::in | ios::out);
    bool found = false;

    while (!file.eof() && !found) {
        streampos pos = file.tellg();
        file.read(reinterpret_cast<char *>(&acc), sizeof(Account));
        if (acc.getAccountNumber() == n) {
            double amount;
            if (option == 1) {
                cout << "Enter amount to deposit: ";
                cin >> amount;
                acc.deposit(amount);
            } else {
                cout << "Enter amount to withdraw: ";
                cin >> amount;
                acc.withdraw(amount);
            }

            file.seekp(pos);
            file.write(reinterpret_cast<char *>(&acc), sizeof(Account));
            cout << "Transaction Completed!\n";
            found = true;
        }
    }
    file.close();
    if (!found)
        cout << "\nAccount Not Found!\n";
}

void displayAll() {
    Account acc;
    ifstream inFile("accounts.dat", ios::binary);
    cout << "\n=== All Account Holders ===\n";
    cout << left << setw(12) << "Acc No"
         << setw(20) << "Name"
         << "Balance\n";
    cout << "-----------------------------------------\n";
    while (inFile.read(reinterpret_cast<char *>(&acc), sizeof(Account))) {
        acc.report();
    }
    inFile.close();
}

void modifyAccount(int n) {
    Account acc;
    fstream file("accounts.dat", ios::binary | ios::in | ios::out);
    bool found = false;

    while (!file.eof() && !found) {
        streampos pos = file.tellg();
        file.read(reinterpret_cast<char *>(&acc), sizeof(Account));
        if (acc.getAccountNumber() == n) {
            acc.showAccount();
            acc.modify();
            file.seekp(pos);
            file.write(reinterpret_cast<char *>(&acc), sizeof(Account));
            found = true;
        }
    }
    file.close();
    if (!found)
        cout << "\nAccount Not Found!\n";
}

void deleteAccount(int n) {
    Account acc;
    ifstream inFile("accounts.dat", ios::binary);
    ofstream outFile("temp.dat", ios::binary);
    bool found = false;

while (!flile.eof() && ! file.read(reainterprit_ anc()eff![].
