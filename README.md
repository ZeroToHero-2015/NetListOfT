# `MyList<T>`

## Temă pentru puncte bonus:

Implementați clasa `MyList<T>`, asemănătoare cu [`List<T>`][listOfT] din .NET Framework, cu următoarele metode și proprietăți:

- `int Count { get; }`             : întoarce numărul de elemente
- `void Add(T item)`               : adaugă un element la sfîrșitul listei
- `T this[int index] { get; set; }`: acces la elementul de la poziția `index`; aruncă `ArgumentOutOfRangeException` dacă indexul e mai mic decît 0 sau mai mare sau egal cu `Count`
- `void Clear()`                   : șterge toate elementele din listă
- `bool Contains(T item)`          : întoarce `true` dacă lista conține `item` și `false` dacă nu
- `void RemoveAt(int index)`       : scoate din listă elementul de la poziția `index` și mută toate elementele de după cu o poziție în față; aruncă `ArgumentOutOfRangeException` dacă indexul e mai mic decît 0 sau mai mare sau egal cu `Count`
- `IEnumerator<T> GetEnumerator()` : implementarea interfeței `IEnumerable<T>`, astfel încît instanțele `MyList<T>` să poată fi folosite cu `foreach`
- `MyList<T> FindAll(Func<T, bool> match)`: întoarce o nouă listă care conține doar elementele din listă pentru care `match` întoarce `true`


[listOfT]: https://msdn.microsoft.com/en-us/library/6sh2ey19%28v=vs.110%29.aspx
