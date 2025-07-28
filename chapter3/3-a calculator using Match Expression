use std::io;

fn main() {
    let mut input = String::new();
    println!("Enter the first number:");
    io::stdin().read_line(&mut input).expect("Failed to read input");
    let num1: f64 = match input.trim().parse() {
        Ok(n) => n,
        Err(_) => {
            println!("Invalid number");
            return;
        }
    };

    input.clear();
    println!("Enter an operator (+, -, *, /):");
    io::stdin().read_line(&mut input).expect("Failed to read input");
    let operator = input.trim().to_string();
    input.clear();
    println!("Enter the second number:");
    io::stdin().read_line(&mut input).expect("Failed to read input");
    let num2: f64 = match input.trim().parse() {
        Ok(n) => n,
        Err(_) => {
            println!("Invalid number");
            return;
        }
    };
    let result = match operator.as_str() {
        "+" => Some(num1 + num2),
        "-" => Some(num1 - num2),
        "*" => Some(num1 * num2),
        "/" => {
            if num2 == 0.0 {
                println!("Error: Division by zero");
                None
            } else {
                Some(num1 / num2)
            }
        },
        _ => {
            println!("Invalid operator");
            None
        }
    };

    if let Some(r) = result {
        println!("Result: {}", r);
    }
}
