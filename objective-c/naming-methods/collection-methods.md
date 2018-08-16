# 集合方法


为了管理集合中的元素，集合应该有这几个方法

- \- (void)addElement:(elementType)anObj;
- \- (void)removeElement:(elementType)anObj;
- \- (NSArray *)elements;

```objectivec
- (void)addLayoutManager:(NSLayoutManager *)obj;
- (void)removeLayoutManager:(NSLayoutManager *)obj;
- (NSArray *)layoutManagers;
```

如果集合是无序的，返回一个NSSet比NSarray更好

如果需要在集合中的特定位置插入元素，使用类似下面的方法

```objectivec
- (void)insertLayoutManager:(NSLayoutManager *)obj atIndex:(int)index;
- (void)removeLayoutManagerAtIndex:(int)index;
```

其他集合方法示例

```objectivec
- (void)addChildWindow:(NSWindow *)childWin ordered:(NSWindowOrderingMode)place;
- (void)removeChildWindow:(NSWindow *)childWin;
- (NSArray *)childWindows;
- (NSWindow *)parentWindow;
- (void)setParentWindow:(NSWindow *)window;
```




{% include links.html %}
