fn main() {
    println!("Multiplication Table (1 to 5):");

    for i in 1..=5 {
        'inner: for j in 1..=10 {
            print!("{:3} ", i * j);

            if i * j > 30 {
                println!("-> breaking 'inner loop at i={}, j={}", i, j);
                break 'inner;
                }
        }
        println!();
    }
}
