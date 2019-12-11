#### *strstr* bildirimi *string.h* dosyası içinde bulunan standart bir C işlevidir.

```
char *strstr(const char *s1, const char *s2);
```

+ İşlev *s1* adresindeki yazı içinde *s2* adresindeki yazıyı arar.
+ Eğer aranılan yazı bulunursa işlevin geri dönüş değeri *s1* yazısı içinde *s2* yazısının başladığı yerin adresidir.
+ Eğ yazı bulunmazsa işlev *NULL* adresine geri döner.

#### İşlevi *mystrstr* ismiyle tanımlayınız.
#### Yazdığınız işlevi aşağıdaki kod ile test edebilirsiniz:

```
#include <stdio.h>
 
char *mystrstr(const char *s1, const char *s2);
 
int main()
{
	char str[] = "You can only be afraid of what you think you know";
	char *p = mystrstr(str, "be");
 
	if (p) {
		printf("bulundu...indis = (%d) (%s)\n", p - str, p);
	}
	else {
		printf("bulunamadi\n");
	}
 
	return 0;
}
```
