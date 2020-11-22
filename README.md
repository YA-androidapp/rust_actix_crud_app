# RustActixCrudApp

actix-web による Web アプリケーション

---

## トップページを表示

```sh
# $ cargo new crudapp
$ cargo init
     Created binary (application) package
$ cargo add actix-web actix-rt thiserror
    Updating 'https://github.com/rust-lang/crates.io-index' index
      Adding actix-web v3.2.0 to dependencies
      Adding actix-rt v1.1.1 to dependencies
      Adding thiserror v1.0.22 to dependencies
$ nano src/main.rs
$ cargo run
```

## CRUD を実装

```sh
$ nano Cargo.toml
# [dependencies] に
# rusqlite = { version = "0.24", features = ["bundled"] }
# serde = { version = "1.0", features = ["derive"] }
# を追記

$ cargo add askama r2d2 r2d2_sqlite
    Updating 'https://github.com/rust-lang/crates.io-index' index
      Adding askama v0.10.5 to dependencies
      Adding r2d2 v0.8.9 to dependencies
      Adding r2d2_sqlite v0.17.0 to dependencies
$ nano src/main.rs
$ nano templates/index.html
$ cargo run
```

---

Copyright (c) 2020 YA-androidapp(https://github.com/YA-androidapp) All rights reserved.
