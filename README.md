
# Variable

-   Mặc định của biến trong Rust là bất biến (immutable)

```
    fn main() {
        let mut x = 10;
        println!("x = {}", x);
        x = 20;
        println!("x = {}", x);

        const HANG_SO: u128 = 100_000_000_000_000_000;
        println!("HANG_SO = {}", HANG_SO)
    }
```

# Shadowing

```
    fn main() {
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

```Scalar Data
    + Interger

    + String
    + Boolean
    + Float


```

```Compound Data

```
