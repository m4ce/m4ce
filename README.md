```rust
impl MatteoCerutti {
    fn profile() -> Self {
        Self {
            alias: "m4ce",
            location: "London",
            email: "matteo.cerutti@hotmail.co.uk"
        }
    }
}

trait Engineer {
    fn interests(&self) -> Vec<&'static str>;

    fn skills(&self) -> Vec<&'static str>;
}

trait Developer {
    fn programming_languages(&self) -> Vec<&'static str>;
}

impl Engineer for MatteoCerutti {
    fn interests(&self) -> Vec<&'static str> {
        vec!["Blockchain", "Crypto", "High frequency trading", "High performance computing", "Cloud computing", "Distributed systems"]
    }

    fn skills(&self) -> Vec<&'static str> {
        vec!["Trading systems design", "Micro-services architecture", "Team leadership", "Troubleshooting"]
    }
}

impl Developer for MatteoCerutti {
    fn programming_languages(&self) -> Vec<&'static str> {
        vec!["Rust", "Java", "C++", "Python", "Shell scripting"]
    }
}
```
