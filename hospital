// BY KARTIKAY JAISWAL - BARCIBAY

#include <stdio.h>

struct Patient {
    char name[30];
    int age;
    char medicalHistory[100];
};    

void addPatient (struct Patient patients[], int* numPatients)
 {
     printf("Enter patient name: "); 
     scanf("%s", &patients[*numPatients].name);

 printf("Enter patient age: ");
 scanf("%d", &patients[*numPatients].age);
 printf("Enter patient medical history: "); 
 scanf("%s", patients[*numPatients].medicalHistory);
(*numPatients)++;
 }

void viewPatient(struct Patient patients[], int numPatients)
{

 for (int i = 0; i < numPatients; i++)
  {
     printf("Patient %d\n", 1+1);
     printf("Name: %s\n", patients[i].name);
     printf("Age: %d\n", patients[i].age);
     printf("Medical History: %s\n", patients[1].medicalHistory);

  }
}

 void deletePatient(struct Patient patients[], int* numPatients)
  {
    int patientNum;
      printf("Enter patient number to delete: ");
      scanf("%d", &patientNum);
      patientNum--;

for(int i = patientNum; i < *numPatients; i++){
    patients[i] = patients[i+1];}
    (*numPatients)--;
  }

int main() 
{
 struct Patient patients [100];

int numPatients = 0;

int choice;

do {

printf("1. Add Patient\n");
printf("2. View Patients\n");
printf("3. Delete Patient\n"); 
printf("4. Exit\n");

printf("Enter your choice: "); 
scanf("%d", &choice);

switch (choice)
 {
    case 1:
         addPatient (patients, &numPatients);
         break;
    case 2:
        viewPatient(patients, numPatients);
        break;
    case 3:
          deletePatient (patients, &numPatients);
          break;
    case 4:
           break;

    default:
         printf("Invalid choice\n");
         break;

 }

   }  while (choice != 4);
return 0;
}
