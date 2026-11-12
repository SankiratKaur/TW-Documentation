# Doxygen

## 1. Introduction

Doxygen is an open-source documentation generator used to create documentation directly from source code.

- It supports languages such as C, C++, Python and Java.
- It extracts information from specially formatted comments.
- It generates documentation in HTML, LaTeX, PDF and other formats.
- It is commonly used for library and API documentation.

## 2. Features of Doxygen

- Automatically generates documentation from source-code comments.
- Documents functions, classes and modules.
- Generates cross-referenced code, call graphs and inheritance diagrams.
- Supports Markdown, LaTeX formulas, Graphviz diagrams and code examples.
- Can be integrated with CI/CD workflows.

## 3. Basic Workflow

The following steps are used to generate documentation:

1. Write specially formatted comments in the source code.
2. Generate a configuration file:

```bash
doxygen -g Doxyfile
```

3. Edit the `Doxyfile` according to project requirements.
4. Generate documentation:

```bash
doxygen Doxyfile
```

5. Open `html/index.html` to view the generated documentation.

## 4. Doxygen Comment Syntax

Doxygen uses special comments to document source code.

**Example (C/C++/Java):**

```cpp
/**
 * \brief Brief description of the function.
 *
 * Longer detailed explanation.
 * \param x Description of the parameter.
 * \return Description of the return value.
 */
int myFunction(int x);
```

Important commands:
- `\brief` – Short description.
- `\param` – Description of a parameter.
- `\return` – Description of the return value.

## 5. Doxygen for Python

Doxygen also supports Python documentation using docstrings.

**Example:**

```python
def foo(bar):
    """
    Brief description.
    More details here.

    :param bar: Bar parameter
    :type bar: int
    :return: Computed value
    :rtype: int
    """
    return bar + 1
```

## 6. Common Doxygen Tags

| Tag | Purpose |
|---|---|
| `\brief` | Short summary |
| `\param` | Parameter description |
| `\return` | Return value description |
| `\author` | Author information |
| `\version` | Version information |
| `\see` | Reference to related items |
| `\note` | Additional information |

## 7. Documenting Classes

Doxygen can document classes and their member functions.

**Example:**

```cpp
/**
 * \class Car
 * \brief Represents a car object.
 *
 * Details about the class.
 */
class Car {
public:
    /**
     * \brief Start the engine.
     * \return True if successful.
     */
    bool startEngine();
};
```

## 8. Grouping and Diagrams

Doxygen provides features to organize code and generate diagrams.

- Logical grouping of related code.
- Call graphs showing function relationships.
- Include diagrams showing file dependencies.
- Graphviz support using `HAVE_DOT = YES` in the Doxyfile.
- Embedding diagrams using `@dot` or PlantUML directives.
- Adding Markdown/HTML tables and images.

## 9. Output Formats

Doxygen supports multiple output formats:

- **HTML:** Documentation for viewing in a browser.
- **LaTeX/PDF:** Printable documentation manuals.
- **RTF:** Rich Text Format.
- **XML:** Structured documentation data.
- **DocBook:** Technical documentation.
- **Man Pages:** Unix manual pages.

Output formats can be configured in the Doxyfile:

```ini
GENERATE_HTML = YES
GENERATE_LATEX = YES
GENERATE_RTF = NO
GENERATE_XML = NO
```

## 10. Best Practices

- Clearly explain the purpose of functions and classes.
- Keep brief and detailed descriptions separate.
- Document all public APIs and modules.
- Use consistent tags and formatting.
- Generate documentation as part of continuous integration.

## 11. Doxygen with Version Control

- Store the `Doxyfile` in the source-code repository.
- Update documentation whenever code changes.
- Review documentation during code reviews.
- Publish generated documentation using GitHub Pages or an internal wiki.

## Conclusion

Doxygen simplifies software documentation by automatically generating reference manuals from source-code comments. It helps developers understand, maintain and collaborate on software projects.