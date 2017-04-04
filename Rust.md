## 特点

- 零开销的抽象
- 转移语义
- 保证内存安全
- 没有数据竞争的线程
- trait 泛型
- 模式匹配
- 类型推断
- 极小运行时
- 高效的C绑定

## 示例

```rust
// 这个代码是可以编辑并且能够运行的
fn main() {
    // 一个简易计算器
    // `+` 或 `-` 意味着加减1
    // `*` 或 `/` 意味着乘除2

    let program = "+ + * - /";
    let mut accumulator = 0;

    for token in program.chars() {
        match token {
            '+' => accumulator += 1,
            '-' => accumulator -= 1,
            '*' => accumulator *= 2,
            '/' => accumulator /= 2,
            _ => { /* 忽略其他 */ }
        }
    }

    println!("程序 \"{}\" 的结果是 {}",
              program, accumulator);
}

```