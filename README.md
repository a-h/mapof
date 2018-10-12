# mapof

A package containing maps which retain the order of the inserted keys.

```go
func ExampleStringToString() {
	m := StringToString()
	m.Add("a", "aa")
	m.Add("b", "bb")
	m.Add("b", "bbb")
	m.Add("c", "c")
	m.Del("c")
	value, ok := m.Get("b")
	fmt.Println(value, ok, m.Keys())
	// Output: bbb true [a b]
}
```
