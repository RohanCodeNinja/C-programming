 C-programming

 #include <stdio.h>

struct student {
    int stdID, Age;
    char Name[20];
    char Add[20];
};

int main() {
    int i;
    struct student s[3];

    for (i = 0; i < 3; i++) {
        printf("Enter the info of student %d:\n", i + 1);
        printf("Enter the ID: ");
        scanf("%d", &s[i].stdID);
        printf("Enter the Name: ");
        scanf("%s", s[i].Name);
        printf("Enter the age: ");
        scanf("%d", &s[i].Age);
        printf("Enter the address: ");
        scanf("%s", s[i].Add);
    }

    for (i = 0; i < 3; i++) {
        printf("Information for student %d:\n", i + 1);
        printf("ID: %d, Name: %s, Age: %d, Address: %s\n", s[i].stdID, s[i].Name, s[i].Age, s[i].Add);
    }

    return 0;
}

