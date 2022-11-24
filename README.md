# ejercicios-prog
~~~

//valores negativos
        while (min < 0) {
            System.out.println("Error. Numero negativo. Volver a intentar");
            System.out.print("minutos: ");
            min = lt.nextInt();
        }
        while (mili < 0) {
            System.out.println("Error. Numero negativo. Volver a intentar");
            System.out.print("milisegundos: ");
            mili = lt.nextInt();
        }
        while (sec < 0) {
            System.out.println("Error. Numero negativo. Volver a intentar");
            System.out.print("segundos: ");
            sec = lt.nextInt();
        }
        
        //valores superiores al límite
        if (mili > 999) {
            sec++;
            mili = mili - 999;
        }
        //sec
        
        if (sec >= 60) {
            min++;
            sec = sec - 60;
        }
~~~
