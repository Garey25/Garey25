import java.util.ArrayList;

public class ArrayListDemo {
    private ArrayList<Integer> numbers;

    // Constructor to initialize the ArrayList
    public ArrayListDemo() {
        numbers = new ArrayList<>();
    }

    // Method to add elements to the ArrayList
    public void addElements() {
        numbers.add(10);
        numbers.add(20);
        numbers.add(30);
        numbers.add(40);
        numbers.add(50);
    }

    // Method to print the ArrayList
    public void printArrayList() {
        System.out.println("ArrayList: " + numbers);
    }

    // Method to access the first element
    public int getFirstElement() {
        return numbers.get(0);
    }

    // Method to modify an element
    public int modifyElement(int index, int newValue) {
        return numbers.set(index, newValue);
    }

    // Method to remove an element
    public int removeElement(int index) {
        return numbers.remove(index);
    }

    // Method to iterate through the ArrayList
    public void iterateArrayList() {
        System.out.println("Iterating over ArrayList:");
        for (int number : numbers) {
            System.out.println(number);
        }
    }

    // Method to calculate the sum of the elements
    public int calculateSum() {
        int sum = 0;
        for (int number : numbers) {
            sum += number;
        }
        return sum;
    }
}



public class Main {
    public static void main(String[] args) {
        // Create an instance of ArrayListDemo
        ArrayListDemo arrayListDemo = new ArrayListDemo();

        // Step 4: Add Elements
        arrayListDemo.addElements();

        // Step 5: Print the ArrayList
        arrayListDemo.printArrayList();

        // Step 6: Access the first element
        int firstNumber = arrayListDemo.getFirstElement();
        System.out.println("First number: " + firstNumber);

        // Step 7: Modify an element
        int oldValue = arrayListDemo.modifyElement(1, 25);
        System.out.println("Old value: " + oldValue);
        arrayListDemo.printArrayList();

        // Step 8: Remove an element
        int removedValue = arrayListDemo.removeElement(3);
        System.out.println("Removed value: " + removedValue);
        arrayListDemo.printArrayList();

        // Step 9: Iterate through the ArrayList
        arrayListDemo.iterateArrayList();

        // Challenge: Calculate the sum of the elements
        int sum = arrayListDemo.calculateSum();
        System.out.println("Sum of elements: " + sum);
    }
}
