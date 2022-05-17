## Razorops CI/CD pipeline demo with Rust

If you have forked this repo, then connect with Razorops to create your demo pipeline by following the below button

[![Connect](https://github.com/razorops-public/images/blob/main/connect_with_github.svg)](https://dashboard.razorops.com/get-github-installation-link-for-org)

[![Build Status](https://api.razorops.com/apps/damp-dew-6277/badge.svg?branch=main)](https://api.razorops.com/apps/damp-dew-6277/workflows)

This is an example code to demonstrate how to create [Rust](https://docs.docker.com/compose/) based pipeline on [Razorops](https://docs.razorops.com/) platform.

This application consists on a basic calculator with sum, multiplication, lcd and gcd operations. 

### Local Setup

#### Prerequisite
* [rust](https://www.rust-lang.org/)
* [cargo](https://crates.io/)

Once you have above software installed. Download/checkout the project and jump to project directory. Then run below commands to build the application:

```bash
cargo build
/target/debug/calc sum 1 2
```
This will create an executable in target/debug directory. Run below commands to play with the calculator:

```bash
./target/debug/calc sum 1 2
3
./target/debug/calc product 2 3 4
24
```

#### Testing 
* To execute tests:
```
cargo test --all
```

### CI/CD pipeline

If you're new to Razorops, feel free to fork this repository and use it to [create a project](https://docs.razorops.com/getting_started/).

`.razorops.yaml` contains the pipeline code to build and execute the tests for this project. To know more about how to write and customize, refer to the [documentation](https://docs.razorops.com). Here is the link of [the pipeline](https://dashboard.razorops.com/apps/damp-dew-6277/workflows) pipeline page.

### License

Copyright (c) 2021 Razorops

Distributed under the MIT License. See the file [LICENSE.md](LICENSE.md).
