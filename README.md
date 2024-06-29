# Sega Genesis Game Project

## Overview
This project is a simple Sega Genesis game developed in C using the Sega Genesis Development Kit (SGDK). The current implementation includes a character that can move within a predefined scenario.

## Features
- Character movement with basic collision detection.
- Scrolling background to simulate movement within a level.
- Simple physics including gravity and jumping.

## Getting Started

### Prerequisites
- [SGDK](https://github.com/Stephane-D/SGDK) (Sega Genesis Development Kit)
- GNU Make
- GCC for M68000

### Setting Up the Development Environment

1. **Install SGDK**:
   Follow the instructions on the [SGDK GitHub page](https://github.com/Stephane-D/SGDK) to set up the development environment on your system.

2. **Clone the Repository**:
   ```sh
   git clone https://github.com/your-username/sega-genesis-game.git
   cd sega-genesis-game
   ```

### Building the Project

To build the project, run the following command in the project directory:
```sh
make -f /path/to/SGDK/makefile.gen
```

### Running the Game

After building the project, you can run the generated ROM file (`out/rom.out`) using a Sega Genesis emulator such as [Kega Fusion](http://segaretro.org/Fusion) or [Gens](http://segaretro.org/Gens).

## How to Play

- **Move Right**: Press the right button.
- **Move Left**: Press the left button.
- **Jump**: Press the C button.

## Troubleshooting

### Common Issues

- **Implicit Declaration of Function**:
  Make sure all necessary functions are correctly declared in the included headers.

- **Undefined Reference to `hintCB`**:
  This may be related to missing interrupt handlers. Ensure that all required interrupt handlers are properly defined.

- **Opening `sega.o`**:
  If you encounter issues with `sega.o`, ensure it is generated correctly and not corrupted. Use `objdump` to inspect the object file if needed.

## Contributing

Feel free to fork the repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [SGDK](https://github.com/Stephane-D/SGDK) for providing the development tools and framework.

---
