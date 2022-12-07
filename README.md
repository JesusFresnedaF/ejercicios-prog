# ejercicios-prog
## BINARY SEARCH ITERATIVO java
~~~
public static int binarySearch(int arr[], int x) {
        int lo = 0, hi = arr.length - 1;

        while (lo <= hi) {
            int mid = lo + (hi - lo) / 2;
            //el número buscado está a la mitad
            if (arr[mid] == x) {
                return mid;
            }
            //el número buscado está por debajo de la mitad
            if (arr[mid] < x) {
                lo = mid + 1;
            } else {//el número buscado está por encima de la mitad
                hi = mid - 1;
            }
        }
        return -1;
    }

    public static void main(String[] args) {
        // TODO code application logic here
        int arr[] = {1, 2, 3, 4, 5};
        int n = arr.length;
        int x = 2;
        int position = binarySearch(arr, x);
        if(position == -1){
            System.out.println("Elemento no existe.");
        }else{
            System.out.println("Elemento encontrado en la posicion: "+position);
        }
    }
~~~

## BURBUJA JUMI
~~~
//declaración de variables
        int nums[] = {5, 4, 3, 2, 1};
        int aux;
        boolean ordenado = false;
        int i = 0;
        
        //metodo burbuja
        while((i < nums.length) || !(ordenado)){
            ordenado = true;
            for (int j = 0; j < nums.length - 1; j++) {
                if(nums[j] > nums[j + 1]){
                    ordenado = false;
                    aux = nums[j];
                    nums[j] = nums[j + 1];
                    nums[j + 1] = aux;
                }
            }
            i++;
        }
        
        //output
        for (int l = 0; l < nums.length; l++) {
            System.out.print(nums[l] + ", ");
            
        }
~~~
