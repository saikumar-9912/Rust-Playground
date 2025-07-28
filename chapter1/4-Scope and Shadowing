fn main() {
    let x = 100;
    println!("Outer x = {}", x);

    {
        let x = x + 50;
        println!("Shadowed x in inner scope = {}", x);

        let y = 200;
        println!("y in inner scope = {}", y);
    } 

    println!("x after inner scope = {}", x); 
}
