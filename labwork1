import java.util.Random;

public class labwork1 {
    public static void main(String[] args) {
        short[] s = new short[10];
        for (int i = 0; i < s.length; i++) {
            s[i] = (short) (3 + 2 * i);
        }

        float[] x = new float[12];
        Random rand = new Random();
        for (int i = 0; i < x.length; i++) {
            x[i] = -5.0f + rand.nextFloat() * 10.0f;
        }

        double[][] a = new double[10][12];

        for (int i = 0; i < s.length; i++) {
            for (int j = 0; j < x.length; j++) {
                double X = x[j];
                if (s[i] == 11) {
                    a[i][j] = (3 - Math.pow(X, Math.sin(X) * (Math.cos(X) + 1))) / Math.PI;
                } else if (s[i] == 5 || s[i] == 7 || s[i] == 13 || s[i] == 15 || s[i] == 17) {
                    a[i][j] = Math.log(Math.pow(Math.exp(X) * (Math.PI / 2 + Math.pow(Math.tan(X), 2)), 2));
                } else {
                    a[i][j] = Math.tan(Math.log(Math.pow(Math.tan(Math.cbrt(X)), 2)));
                }
            }
        }

        System.out.println("Массив s:");
        for (short value : s) {
            System.out.print(value + " ");
        }
        System.out.println("\n");

        System.out.println("Массив x:");
        for (float value : x) {
            System.out.printf("%.3f ", value);
        }
        System.out.println("\n");

        System.out.println("Массив a (10x12):");
        for (int i = 0; i < a.length; i++) {
            for (int j = 0; j < a[i].length; j++) {
                System.out.printf("%10.3f ", a[i][j]);
            }
            System.out.println();
        }
    }
}
