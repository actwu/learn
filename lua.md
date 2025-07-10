<link rel="preload" as='style' href="https://actwu.github.io/md2.css"/>
<link rel="stylesheet" href="https://actwu.github.io/md2.css"/>
<script src="https://cdn.jsdelivr.net/gh/iselang/iselang.github.io@main/num.min.js"></script>
<script>
app('Learn-Lua'); fav(3);
</script>

- **while loop**: Executes a block repeatedly while a condition is true. Syntax:
  ```lua
  while condition do
    -- statements
  end
  ```
  Example printing numbers 10 to 19:
  ```lua
  a = 10
  while a < 20 do
    print(a)
    a = a + 1
  end
  ```
  The loop stops when the condition is false[1][3][7].

- **function (func)**: Defined using `function` keyword. Example:
  ```lua
  function greet(name)
    print("Hello " .. name)
  end
  greet("World")
  ```

- **if statement / ternary**: Lua uses `if ... then ... elseif ... else ... end` for conditionals. Lua does not have a built-in ternary operator, but you can simulate it with `and`/`or` expressions:
  ```lua
  local result = condition and value_if_true or value_if_false
  ```
  Note: This only works reliably if `value_if_true` is not false or nil[6][8]. Example:
  ```lua
  local max = (a > b) and a or b
  ```

- **delay**: Lua itself does not have a built-in `delay` function. In environments like Roblox or embedded systems, you use functions like `task.wait(seconds)` or platform-specific delay functions. For example, in Roblox Lua:
  ```lua
  task.wait(2) -- delays for 2 seconds
  ```
  
- **for loop**: Used for iterating over ranges or collections:
  ```lua
  for i = 1, 5 do
    print(i)
  end
  ```
  or iterating arrays:
  ```lua
  local arr = {10, 20, 30}
  for i, v in ipairs(arr) do
    print(i, v)
  end
  ```
  Lua also supports generic for loops over tables[4].

- **var**: Lua uses dynamically typed variables declared simply by assignment; no explicit `var` keyword:
  ```lua
  x = 10
  name = "Lua"
  ```
  Variables are global by default unless declared `local`:
  ```lua
  local x = 5
  ```

