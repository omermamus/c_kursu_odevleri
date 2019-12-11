#### Sizce aşağıdaki kodda tanımlanan *func* isimli işlev ne yapıyor?

```
#include <stdio.h>

void func(int x > 1)
{
	if (x) 
		func(x / 2);
	putchar('0' + x % 2);	
}
```
