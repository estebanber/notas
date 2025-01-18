# Ejercicio Live coding
Ejercicio tomado en entrevista de Qbica el día 20/11/2024.
Implementar funciones memcpy y strnlen

```c
#include <assert.h>

#include <stdio.h>
#include <string.h>

// To get started, click on the green "Fork this" button above

// Rules:
//  - Can't use generative tools
//  - Can't use help forums (stackoverflow.com and such)
//  - Can use technical references (cplusplus.com, cppreference.com, man7.org, etc)
//  - Unaligned accesses are not permitted
//  - Can assume a little endian architecture
//  - Can use the C standard lib (except for memcpy and strnlen)
//  - You can use the "Run" button as many times as needed

void *my_memcpy(void *restrict dest, const void *restrict src, size_t count)
{
	char *d = dest;
	char *s = (char*)src;
	size_t n = 0;
	while(n<count)
	{
		*d++ = *s++;
		n++;
	}
	return dest;
}

size_t my_strnlen(const char *s, size_t max)
{
	size_t n = 0;
	char curr = *s;
	while(n < max && curr != 0 )
	{
		n++;
		s++;
		curr = *s;
	}
	return n;
}

// The contents of the main function cannot be modified
int main()
{
	char buffer[32] = {};
	const char *str = "Hello, world! This is a test";

	int str_len = my_strnlen(str, 23);

	char *buf = my_memcpy(buffer, str, str_len);



	assert(23 == my_strnlen(buf, 24));
	assert(23 == str_len);
	assert(memcmp(str, buffer, str_len) == 0);
	assert(buf == &buffer[0]);
	assert(strcmp("Hello, world! This is a", buf) == 0);
	printf("TEST PASSED!\n");
	return 0;
}
```
