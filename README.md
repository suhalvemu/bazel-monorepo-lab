# bazel-monorepo-lab
Bazel Monorepo lab
# bazel-monorepo-lab

A sample monorepo demonstrating multi-language builds using [Bazel](https://bazel.build/).

## Features

- **Go, Python, and Java** project support
- Modern [bzlmod](https://bazel.build/docs/bzlmod) dependency management
- Example Bazel rules for each language
- Simple, reproducible builds

## Project Structure

```
.
├── java_app/      # Java application
├── python_app/    # Python application
├── MODULE.bazel   # Bazel module definition
├── WORKSPACE      # Bazel workspace file
└── ...
```

## Getting Started

1. **Install Bazel:**  
   [Follow the official instructions](https://bazel.build/install).

2. **Build all projects:**
   ```sh
   bazel build //...
   ```

3. **Run the Java app:**
   ```sh
   bazel run //java_app:java_app
   ```

4. **Run the Python app:**
   ```sh
   bazel run //python_app:python_app
   ```

## Adding Dependencies

- Edit `MODULE.bazel` to add new Bazel dependencies.
- Use language-specific rules (e.g., `rules_go`, `rules_python`, `rules_java`).

## License

MIT