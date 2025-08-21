#include <stdio.h>
#include <string.h>

int main() {
    char str[] = "Hello World";
    printf("Length = %lu\n", strlen(str));
    return 0;
}

#include <stdio.h>
#include <string.h>

int main() {
    char src[] = "C Programming";
    char dest[50];

    strcpy(dest, src);
    printf("Copied String: %s\n", dest);

    return 0;
}

#include <stdio.h>
#include <string.h>

int main() {
    char src[] = "Hello World";
    char dest[20];

    strncpy(dest, src, 5);   // Copy first 5 chars
    dest[5] = '\0';          // Add null terminator
    printf("First 5 chars: %s\n", dest);

    return 0;
}

#include <stdio.h>
#include <string.h>

int main() {
    char str1[50] = "Hello ";
    char str2[] = "World";

    strcat(str1, str2);
    printf("Concatenated: %s\n", str1);

    return 0;
}

#include <stdio.h>
#include <string.h>

int main() {
    char str1[50] = "Hello ";
    char str2[] = "World!!!";

    strncat(str1, str2, 5);  // Append only first 5 chars
    printf("Concatenated: %s\n", str1);

    return 0;
}

#include <stdio.h>
#include <string.h>

int main() {
    char str1[] = "Hello";
    char str2[] = "World";

    if (strcmp(str1, str2) == 0)
        printf("Strings are equal\n");
    else
        printf("Strings are different\n");

    return 0;
}
#include <stdio.h>
#include <string.h>

int main() {
    char str1[] = "HelloWorld";
    char str2[] = "HelloC";

    if (strncmp(str1, str2, 5) == 0)
        printf("First 5 characters are equal\n");
    else
        printf("First 5 characters are different\n");

    return 0;
}

#include <stdio.h>
#include <string.h>

int main() {
    char str[] = "Hello World";
    char *ptr = strchr(str, 'o');

    if (ptr)
        printf("Found 'o' at position: %ld\n", ptr - str);
    else
        printf("Character not found\n");

    return 0;
}

#include <stdio.h>
#include <string.h>

int main() {
    char str[] = "Hello World";
    char *ptr = strrchr(str, 'o');

    if (ptr)
        printf("Last 'o' at position: %ld\n", ptr - str);
    else
        printf("Character not found\n");

    return 0;
}

#include <stdio.h>
#include <string.h>

int main() {
    char str[] = "I love C programming";
    char *ptr = strstr(str, "C");

    if (ptr)
        printf("Found substring at position: %ld\n", ptr - str);
    else
        printf("Substring not found\n");

    return 0;
}

