## Energy Web - Rust Developer recruitment task

Hey there!

Not so long ago we decided to create a catalogue of our favorite movies (./src/db.json) as json. It is hard to find things there, so we would like to build an algorithm to make it easier.

## Before start
1. Please remove `.git` folder and initialize your own repository using this repository as a starting point
2. Please install all dependencies using `cargo build`

## TODO'S
1. Write an algorithm that would help us find the right movie: 
  * If we provide genres [Comedy, Fantasy, Crime] then the top hits should be movies that have all three of them, then there should be movies that have one of [Comedy, Fantasy], [Comedy, Crime], [Fantasy, Crime] and then those with Comedy only, Fantasy only and Crime only. Similarly applies when the requested array of genres is shorter.

  * Of course we don't want to have duplicates.

  * If we provide an empty list, then we should get a single random movie. (return type should be a array with single movie)

2. The algorithm needs to be as efficient as possible, so please also provide its time complexity using "Big O" notation with some explanation how you've calculated it. 

To make it easier we've also provided a set of tests to make sure your solution works as expected. You can find them in `./tests/movies.rs`. To run them use:
```bash
cargo test
```

### Rules
* You may use external crates of your choice, such as `serde`, in order read the `db.json` file. You may need to adjust the types to facilitate deserialization.
* Please **do not** use an external crate for the movie algorithm.
* We require code in git repository
* All tests needs to pass