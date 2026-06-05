#include <stdio.h>

int main() {

    char s[100];
    int i;

    printf("Nhap chuoi: ");
    gets(s);

    // Chuyen chu hoa thanh chu thuong
    for(i = 0; s[i] != '\0'; i++) {

        if(s[i] >= 'A' && s[i] <= 'Z') {

            s[i] = s[i] + 32;
        }
    }

    printf("Chuoi thuong: %s", s);

    return 0;
}
