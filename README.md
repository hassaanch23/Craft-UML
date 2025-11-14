# Craft-UML

[![Java](https://img.shields.io/badge/Java-22-orange.svg)](https://www.oracle.com/java/)
[![JavaFX](https://img.shields.io/badge/JavaFX-22.0.1-blue.svg)](https://openjfx.io/)
[![Maven](https://img.shields.io/badge/Maven-3.8.5-red.svg)](https://maven.apache.org/)

Craft-UML is a feature-rich desktop application built using Java and JavaFX for designing, editing, and managing UML diagrams. This project was developed as part of the Software Construction and Development course during the 5th semester of Bachelor's in Software Engineering.

The application provides an intuitive interface for creating professional UML diagrams, including Class Diagrams and Use Case Diagrams, with support for exporting diagrams and generating boilerplate code from class diagrams.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [How to Run](#how-to-run)
- [Building the Project](#building-the-project)
- [Running Tests](#running-tests)
- [Usage](#usage)
- [Contributing](#contributing)
- [Contributors](#contributors)
- [License](#license)
- [Acknowledgments](#acknowledgments)
- [Contact](#contact)

## Features

### UML Class Diagrams
- **Create and Edit Classes**: Add classes with attributes and methods
- **Relationships**: Support for associations, generalizations, compositions, aggregations, and other UML relationships
- **Interface Support**: Create and manage interfaces
- **Code Generation**: Generate boilerplate Java code from class diagrams
- **Full CRUD Operations**: Edit and delete existing classes and relationships

### UML Use Case Diagrams
- **Actors and Use Cases**: Add and manage actors and use cases
- **Rich Relationships**: Support for include, exclude, association, and generalization relationships
- **Flexible Editing**: Modify or remove elements easily
- **Interactive Design**: Drag-and-drop interface for easy diagram creation

### Export and Save Functionality
- **Image Export**: Save diagrams as PNG or JPG for presentations and documentation
- **Custom File Format**: Save diagrams in a proprietary format for later editing within Craft-UML
- **Persistence**: Serialize and deserialize diagram data using JSON

### User Experience
- **Intuitive UI**: Clean and user-friendly interface built with JavaFX
- **Error Handling**: Robust validation and user feedback for invalid operations
- **Responsive Design**: Maximized window for better workspace utilization

## Technologies Used

- **Java 22**: Core programming language
- **JavaFX 22.0.1**: GUI framework for building the desktop application
- **Maven**: Build automation and dependency management
- **JUnit 5**: Unit testing framework
- **Mockito**: Mocking framework for tests
- **TestFX**: JavaFX testing framework
- **Jackson**: JSON serialization/deserialization
- **Apache PDFBox**: PDF handling capabilities
- **ControlsFX**: Enhanced JavaFX controls

## Prerequisites

Before running this application, ensure you have the following installed:

- **Java Development Kit (JDK) 17 or higher** (JDK 22 recommended)
  - Download from [Oracle](https://www.oracle.com/java/technologies/downloads/) or [OpenJDK](https://openjdk.org/)
- **Maven 3.8+** (or use the included Maven wrapper)
- **JavaFX SDK** (included as Maven dependencies)

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/hassaanch23/Craft-UML.git
   cd Craft-UML
   ```

2. **Verify Java installation**:
   ```bash
   java -version
   ```
   Ensure the version is 17 or higher.

3. **Make the Maven wrapper executable** (Linux/macOS):
   ```bash
   chmod +x mvnw
   ```

## How to Run

### Using Maven (Recommended)

Run the application directly using Maven:

```bash
./mvnw clean javafx:run
```

On Windows:
```cmd
mvnw.cmd clean javafx:run
```

### Using an IDE

1. **Import the project** into your preferred IDE (IntelliJ IDEA, Eclipse, or NetBeans)
2. **Wait for Maven** to download dependencies
3. **Run** the `HelloApplication` class located at:
   ```
   src/main/java/org/example/craftuml/HelloApplication.java
   ```

### Manual Compilation

```bash
# Compile the project
./mvnw clean compile

# Run the application
./mvnw javafx:run
```

## Building the Project

To build the project and create a distributable package:

```bash
./mvnw clean package
```

This will compile the code, run tests, and create a JAR file in the `target/` directory.

## Running Tests

The project includes comprehensive unit tests for models, business logic, and UI components.

### Run all tests:
```bash
./mvnw test
```

### Run tests with coverage:
```bash
./mvnw clean test
```

### Run specific test classes:
```bash
./mvnw test -Dtest=ClassDiagramTest
```

## Usage

1. **Launch the application** using one of the methods described above
2. **Create a new diagram**:
   - Select the type of diagram you want to create (Class Diagram or Use Case Diagram)
   - Use the toolbar to add elements to your diagram
3. **Edit elements**:
   - Click on elements to select them
   - Use the context menu or property panel to modify attributes
4. **Create relationships**:
   - Select the relationship type from the toolbar
   - Click on the source element, then the target element
5. **Save your work**:
   - Use File → Save to save in the custom format
   - Use File → Export to save as PNG or JPG
6. **Generate code** (Class Diagrams only):
   - Use the code generation feature to export Java class templates

## Contributing

Contributions are welcome! If you'd like to contribute to Craft-UML, please follow these steps:

1. **Fork the repository**
2. **Create a new branch**:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Make your changes** and commit them:
   ```bash
   git commit -m "Add: Description of your changes"
   ```
4. **Push to your branch**:
   ```bash
   git push origin feature/your-feature-name
   ```
5. **Open a Pull Request** with a clear description of your changes

### Code Style
- Follow standard Java coding conventions
- Write clear, descriptive commit messages
- Add unit tests for new features
- Ensure all tests pass before submitting a PR

## Contributors

This project is maintained and developed by:

- **Muhammad Hassaan** ([@hassaanch23](https://github.com/hassaanch23)) - *Creator and Lead Developer*

Special thanks to all contributors who have helped improve this project!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details (if applicable).

## Acknowledgments

- This project was developed as part of the **Software Construction and Development** course
- Thanks to the **Bachelor's in Software Engineering** program for providing the foundation and learning opportunity
- Built with [JavaFX](https://openjfx.io/) - an excellent framework for building rich desktop applications
- Inspired by professional UML modeling tools

## Contact

For questions, suggestions, or feedback, please reach out:

- **GitHub**: [@hassaanch23](https://github.com/hassaanch23)
- **Repository**: [Craft-UML](https://github.com/hassaanch23/Craft-UML)
- **Issues**: [Report a bug or request a feature](https://github.com/hassaanch23/Craft-UML/issues)

---

⭐ If you find this project helpful, please consider giving it a star on GitHub!
