fn main() {
    let x = 10;

    let reference_to_x = &x;

    println!("Value of x: {}", x);
    println!("Reference to x (borrowed): {}", reference_to_x);

    println!("Dereferenced value: {}", *reference_to_x);

    let mut y = 20;
    {
        let mutable_ref = &mut y;
        *mutable_ref += 5;
        println!("Inside block - Modified value via mutable reference: {}", mutable_ref);
    }

    println!("After modification, y: {}", y);
}
