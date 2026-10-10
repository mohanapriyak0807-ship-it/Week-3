# Week-3

import java.util.Scanner;

class Week3 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String[] products = {
            "Running Shoes",
            "Sports Shoes",
            "Leather Belt",
            "Sports Cap"
        };

        System.out.print("Enter product name: ");
        String search = sc.nextLine();

        boolean found = false;

        for (String product : products) {
            if (product.toLowerCase().contains(search.toLowerCase())) {
                System.out.println("Product Found: " + product);
                found = true;
            }
        }

        if (!found) {
            System.out.println("Product not found!");
        }

        sc.close();
    }
}
