ssh-keygen -t ed25519 -C "gowdanjan18@gmail.com"
 cat ~/.ssh/id_ed25519.pub
 eval "$(ssh-agent -s)"
 ssh-add ~/.ssh/id_ed25519
 ssh -T git@github.com
 mkdir demo
cd demo
git init
echo "Hello Git" > a.txt
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/AnjanC18/demo.git
git push -u origin main


  public class BubbleSortExample {

    public static void main(String[] args) {

        int[] arr = {5, 2, 9, 1, 6};

        int n = arr.length;

        // Bubble Sort
        for (int i = 0; i < n - 1; i++) {

            for (int j = 0; j < n - 1 - i; j++) {

                if (arr[j] > arr[j + 1]) {

                    // Swap
                    int temp = arr[j];
                    arr[j] = arr[j + 1];
                    arr[j + 1] = temp;
                }
            }
        }

        // Print Sorted Array
        System.out.println("Sorted Array:");
        for (int num : arr) {
            System.out.print(num + " ");
        }
    }
}
