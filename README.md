# Craft-UML

Craft-UML is a desktop application for designing, editing, and exporting UML diagrams. Built with modern Java and JavaFX libraries, the app supports class diagrams, use-case diagrams, relationships, export options, and basic code generation from diagrams.

**Repository snapshot:** a Java (modular) project using Maven and JavaFX with a collection of unit and UI tests (TestFX).

**Highlights:** intuitive editor for UML diagrams, export to image, save/load projects, and diagram-to-code boilerplate generation.

## Features

- **UML Class Diagrams:** create classes, attributes, methods, and common relationships (association, aggregation, composition, inheritance).
- **UML Use Case Diagrams:** add actors, use cases, and relationships (include, extend, association).
- **Edit & Manage Diagrams:** move, rename, modify, and delete diagram elements.
- **Exporting:** save diagrams as PNG/JPG for sharing or documentation.
- **Persistence:** save and load diagrams in the project's custom format for later editing.
- **Code Generation:** export basic boilerplate code from class diagrams.
- **Tests:** includes unit tests and UI tests using TestFX and JUnit.

## Technology Stack

- **Language:** Java (source/target set to Java 22 in `pom.xml`)
- **UI:** JavaFX (FXML, `javafx-controls`, `javafx-fxml`)
- **UI Tooling/Libraries:** ControlsFX, TilesFX, Ikonli, FormsFX, ValidatorFX
- **Build:** Maven (wrapper available: `mvnw` / `mvnw.cmd`)
- **Testing:** JUnit 5, TestFX, Mockito

## Prerequisites

- Java JDK 22 (or compatible Java 22+ distribution)
- Git (to clone the repository)
- (Optional) An IDE with JavaFX support (IntelliJ IDEA, Eclipse, VS Code with extensions)

Note: The project includes the Maven wrapper (`mvnw` / `mvnw.cmd`), so a local Maven installation is optional.

## Installation & Running (Development)

1. Clone the repository:

```powershell
Git clone https://github.com/hassaanch23/Craft-UML.git
cd "Craft-UML"
```

2. Run the application using the Maven wrapper (Windows PowerShell):

```powershell
.\mvnw.cmd javafx:run
```

Or with a local Maven installation:

```powershell
mvn javafx:run
```

Alternatively, open the project in your IDE and run the `org.example.craftuml.HelloApplication` main module/class.

## Building a distributable

Package the application (creates the jar or build artifacts according to the Maven configuration):

```powershell
.\mvnw.cmd package
# or
mvn package
```

Depending on the `javafx-maven-plugin` configuration and your environment, you may also produce a platform image using the plugin's jlink/jpackage capabilities.

## Running Tests

Run unit and UI tests with:

```powershell
.\mvnw.cmd test
# or
mvn test
```

Note: UI tests (TestFX) may require a graphical environment and compatible JavaFX setup.

## Project Structure

Top-level layout (relevant folders/files):

- `src/main/java/org/example/craftuml/` — application source including `HelloApplication.java`, controllers, business logic, models, and UI helper classes.
- `src/main/resources/org/example/craftuml/` — FXML views, CSS, and images used by the UI.
- `src/test/java/TEST/` — unit and UI tests for the application features.
- `pom.xml` — Maven project file (Java version, dependencies, and `javafx-maven-plugin` configuration).
- `mvnw`, `mvnw.cmd` — Maven wrapper scripts for cross-machine consistency.

## Contributing

- Contributions, bug reports, and feature requests are welcome. Please open an issue or submit a pull request.
- When contributing, prefer small, focused changes with a clear description and, if applicable, test coverage.

## Known Notes & Tips

- The `pom.xml` targets Java 22; ensure your `JAVA_HOME` points to a Java 22 JDK for best compatibility.
- If you have problems running JavaFX, ensure JavaFX modules are available or let the `javafx-maven-plugin` download them.
- UI tests may need a display; on headless CI, configure a virtual frame buffer or skip TestFX UI tests.

## Authors / Maintainers

- Muhammad Hassaan — `@hassaanch23`



---


