# Tutorial lisp

This is a repository with the base for building your own lisp Youtube series.

Each branch should have the code for the end of each video.

## Instructions

* To build the lisp you need the C compiler installed, to test if you have it on your machine just run the command:
```
cc --version
```

* If you don't have the compiler installed use the follow the instructions:
```
# Ubuntu:
sudo apt-get install build-essential

# Fedora
su -c "yum groupinstall development-tools"

# Mac
xcode-select --install

# Windows
# Install MinGW https://www.mingw-w64.org/ and add it to the path.
```

* If you already have the compiler installed just go to the project folder and use the command:

```
make all
./lisp
```

* This should open a simple REPL that will echo everything that you type in there. This also have a history, so you can navigate within it using up arrow and down arrow.

## Project structure

The project structure is very simple with the bare minimum for our lisp language. It contains the following structure:
```
.
├── README.md -- Instructions for running the code and general docs
├── makefile -- Used to build our application
└── source -- Folder where we put our source files
    ├── main.c -- Application entry point
    ├── mpc.c -- A library for parser combinator
    └── mpc.h -- Parser combinator headers
```

