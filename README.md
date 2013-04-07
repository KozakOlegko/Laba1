Laba1
=====
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Laba1
{
    class Program
    {
        class CubicMatrix
        {
            public CubicMatrix() { }
            private int[,][] M;
            //5 3 4
            public void InputMatrix()
            {
                M = new int[5, 3][];
                M[0, 0] = new int[4] { 1, 2, 3, 4 };
                M[0, 1] = new int[4] { 11, 12, 33, 78 };
                M[0, 2] = new int[4] { 21, 42, 53, 74 };

                M[1, 0] = new int[4] { 31, 22, 13, 8 };
                M[1, 1] = new int[4] { 41, 32, 33, 28 };
                M[1, 2] = new int[4] { 51, 62, 93, 9 };


                M[2, 0] = new int[4] { 71, 92, 43, 5 };
                M[2, 1] = new int[4] { 6, 82, 73, 75 };
                M[2, 2] = new int[4] { 10, 20, 30, 40 };


                M[3, 0] = new int[4] { 104, 998, 453, 865 };
                M[3, 1] = new int[4] { 657, 987, 346, 976 };
                M[3, 2] = new int[4] { 874, 423, 342, 243 };


                M[4, 0] = new int[4] { 154, 765, 353, 533 };
                M[4, 1] = new int[4] { 109, 236, 332, 543 };
                M[4, 2] = new int[4] { 123, 246, 385, 853 };


            }
            public void Output()
            {
                Console.WriteLine("масив:");
                for (int k = 0; k < 5; k++)
                    for (int i = 0; i < 3; i++)
                        for (int j = 0; j < 4; j++)
                            Console.WriteLine("M[" + (k + 1) + ", " + (i + 1) + ", " + (j + 1) + "]=" + M[k, i][j]);

            }

           static void Main(string[] args)
            {
                CubicMatrix CM = new CubicMatrix();
                CM.InputMatrix();
                CM.Output();
               // CM.GetFRONT();
                //CM.FuncVector();
                Console.ReadKey();
            }
        }
    }
}
