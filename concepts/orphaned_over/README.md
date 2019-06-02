# Quick Reference

An orphaned Over is an Over that does not author an Opinion that affects
the composed Stage's result. In short, it's an `over` specifier that
points to nothing. Check out the [usda folder](usda) for a better idea
of what that looks like, if needed.


```cpp
for (auto const &prim : stage->TraverseAll()) {
    if (!prim.IsDefined()) {
        std::cout << prim.GetPath() << std::endl;
    }
}
```

```python
print(list(prim for prim in stage.TraverseAll() if not prim.IsDefined()))
```