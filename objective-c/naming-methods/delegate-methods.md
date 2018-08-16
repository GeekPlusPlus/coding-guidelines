# 代理方法

以发送消息的对象开始

省略了前缀的类名和首字母小写

```objectivec
- (BOOL)tableView:(NSTableView *)tableView shouldSelectRow:(int)row;
- (BOOL)application:(NSApplication *)sender openFile:(NSString *)filename;
```

以发送消息的对象开始的规则不适用下列两种情况

只有一个sender参数的方法

```objectivec
- (BOOL)applicationOpenUntitledFile:(NSApplication *)sender;
```

响应notification的方法（方法的唯一参数就是notification）

```objectivec
- (void)windowDidChangeScreen:(NSNotification *)notification;
```

使用单词 did 和 will 来通知delegate

- did 表示某些事已发生
- will 表示某些事将要发生

```objectivec
- (void)browserDidScroll:(NSBrowser *)sender;
- (NSUndoManager *)windowWillReturnUndoManager:(NSWindow *)window;
```

询问delegate是否可以执行某个行为时可以使用 did 或 will，不过 should 更完美  

```objectivec
- (BOOL)windowShouldClose:(id)sender;
```




{% include links.html %}
