**Répète de 1 à n fois le template ``$"{i} sheep..."`` et assemble en chaîne de caractères**

```c#
using System.Linq;

string result = string.Concat(Enumerable.Range(1, n).Select(i => $"{i} sheep..."));
```

---

**Fusionne deux array puis calcule la somme des éléments du tableau fusionné**
```c#
using System.Linq;

int result = Enumerable.Concat(arr1, arr2).ToArray().Sum();
```

---

**Filtre les éléments d'un tableau en fonction d'une condition**
```c#
using System.Linq;

object[] result = arr.Where((e, i) => i%2 == 0).ToArray();
```

--

**Créé un tableau de n éléments ayant pour valeur leur index**
```c#
using System.Linq;

int[] result = Enumerable.Range(1, n).ToArray();
```

---

**Compte combien de fois apparaît la lettre c dans la string**
```c#
using System.Linq;

int result = str.Count(c => c.ToString() == 'c');
```

---

**Ecritures raccourcies d'un ``switch``**
```c#
string s = i switch {
	1 => "One",
	2 => "Two",
	3 => "Three",
	_ => "Default",
}


//  Avec expression d'une condition
switch (average) {
    case int d when d >= 90: return 'A';
    case int d when d >= 80: return 'B';
    case int d when d >= 70: return 'C';
    case int d when d >= 60: return 'D';
    default: return 'F';
}
```

---

**Somme des éléments du tableau x avec conversion en Int32 de chacun des éléments**
```c#
using System.Linq;

int result = x.Sum(ToInt32);
```
---