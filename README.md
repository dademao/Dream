/*7、    综合应用题
 编写九九乘法表
*/
#include<stdio.h>
int main ()
{
    int n = 1 , m = 10 ;
    for ( int i = 1 ; i < 10 ; i ++ , n ++ )
    {
        printf ("%d * %d = %d", n , i , n * i );
        while ( n != i )//这里以两个数相等作为结束的条件
        {
            n ++ ;
            printf("\t%d * %d = %d", n , i , n * i );
        }
        n = 0 ;//因为在while循环里面n的值已经不在是1 了，还有就是for循环里面有一个n++，所以这里的n要为零
        printf ("\n");//经过一轮循环之后要换行
    }
    return 0 ;
}
