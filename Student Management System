import java.util.ArrayList;
import java.util.Scanner;

class Student {
    String name;
    int rollNo;
    String grade;

    Student(String name, int rollNo, String grade) {
        this.name = name;
        this.rollNo = rollNo;
        this.grade = grade;
    }
}

public class StudentManagementSystem {
    static ArrayList<Student> students = new ArrayList<>();
    static Scanner scanner = new Scanner(System.in);

    public static void main(String[] args) {
        while (true) {
            System.out.println("1. Add Student\n2. View Students\n3. Exit");
            int choice = scanner.nextInt();
            scanner.nextLine();

            switch (choice) {
                case 1:
                    addStudent();
                    break;
                case 2:
                    viewStudents();
                    break;
                case 3:
                    System.exit(0);
                default:
                    System.out.println("Invalid choice!");
            }
        }
    }

    static void addStudent() {
        System.out.print("Enter name: ");
        String name = scanner.nextLine();
        System.out.print("Enter roll no: ");
        int rollNo = scanner.nextInt();
        scanner.nextLine(); 
        System.out.print("Enter grade: ");
        String grade = scanner.nextLine();

        students.add(new Student(name, rollNo, grade));
        System.out.println("Student added!");
    }

    static void viewStudents() {
        for (Student student : students) {
            System.out.println("Name: " + student.name + ", Roll No: " + student.rollNo + ", Grade: " + student.grade);
        }
    }
}
