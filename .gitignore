#include <stdio.h>

#define MOD 12345
#define MAX_N 10000

int main() {
    int n;
    printf("Введіть довжину послідовності n: ");
    scanf("%d", &n);

    if (n < 1 || n >= MAX_N) {
        printf("Неприпустиме значення n\n");
        return 1;
    }

    int dp[MAX_N];
    dp[0] = 1;     
    dp[1] = 2;     
    dp[2] = 4;    

    for (int i = 3; i <= n; i++) {
        dp[i] = (dp[i-1] + dp[i-2] + dp[i-3]) % MOD;
    }

    printf("Кількість шуканих послідовностей: %d\n", dp[n]);
    return 0;
}
