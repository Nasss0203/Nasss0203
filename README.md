
# Variable

-   Mặc định của biến trong Rust là bất biến (immutable)

```fn main() {
        let mut x = 10;
        println!("x = {}", x);
        x = 20;
        println!("x = {}", x);

        const HANG_SO: u128 = 100_000_000_000_000_000;
        println!("HANG_SO = {}", HANG_SO)
    }
```

# Shadowing

```fn main() {
        //Shadowing
        let outer = 10;
        {
            let inner = 200;
            println!("inner = {}", inner);
            let outer = 300;
            println!("outer = {}", outer);
        }
        println!("outer = {}", outer);
    }
```

# Data Types

## Scalar Data

| Độ dài (bits) | Có dấu | Không dấu |
| ------------- | ------ | --------- |
| 8-Bit         | i8     | u8        |
| 16-Bit        | i16    | u16       |
| 32-Bit        | i32    | u32       |
| 64-Bit        | i64    | u64       |
| 128-Bit       | i128   | u128      |
| arch-Bit      | isize  | usize     |

### Interger

```fn main() {
    let a = 111_111; //Demicals
    let b = 0xff; //Hex
    let c = 0o77; //Octal
    let d = 0b1111_000; //Binary
    let e = b'A'; //Byte
    println!("a = {}", a);
    println!("b = {}", b);
    println!("c = {}", c);
    println!("d = {}", d);
    println!("e = {}", e);
}
```

### Float

```fn main() {
    let _f = 2.0;
    let _g: f32 = 3.0;

    let sum = 3 + 4;
    let subtraction = 5 - 4;
    let multiplication = 3 * 5;
    let division = 40.4 / 20.4;
    let remainder = 43 % 4;
    println!("sum = {}", sum);
    println!("subtraction = {}", subtraction);
    println!("multiplication = {}", multiplication);
    println!("division = {}", division);
    println!("remainder = {}", remainder);
}
```

### String

### Boolean

## Compound Data
