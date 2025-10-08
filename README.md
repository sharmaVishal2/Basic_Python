# Basic_Python
Python pg
<!DOCTYPE html>
<html lang="en" data-theme="dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Introduction to Python Programming</title>
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/prism/1.29.0/themes/prism-tomorrow.min.css">
</head>
<body>
    <div id="blob"></div>
    <div id="blur"></div>

 <nav>
        <div class="logo">🐍 PyLearn</div>
        <div class="nav-links">
            <a href="#variables">Variables</a>
            <a href="#operators">Operators</a>
            <a href="#blocks">Blocks</a>
            <a href="#datatypes">Data Types</a>
            <button id="darkModeToggle">☀️</button>
        </div>
    </nav>

    <header class="hero">
        <div class="hero-content">
            <h1>Introduction to Python Programming</h1>
            <p class="subtitle">Your first step into the world of Python. Learn the essentials: Variables, Operators, Data Types, and Code Blocks.</p>
            <a href="#variables" class="cta-button">Start Learning</a>
        </div>
    </header>

  <main>
        <section id="variables">
            <h2>Python Variables 📦</h2>
            <div class="section-content">
                <p>In Python, a variable is a symbolic name that acts as a reference or pointer to an object in memory. You create a variable the moment you first assign a value to it.</p>
                
                <h3>Naming Rules and Conventions:</h3>
                <ul>
                    <li>Must start with a letter (a-z, A-Z) or an underscore (_).</li>
                    <li>The rest of the name can contain letters, numbers (0-9), and underscores.</li>
                    <li>Variable names are <strong>case-sensitive</strong> (`age`, `Age`, and `AGE` are three different variables).</li>
                    <li>The standard convention in Python is to use <strong>snake_case</strong> for variable names (e.g., `my_first_name`).</li>
                </ul>

                <h3>Dynamic Typing:</h3>
                <p>Python is <strong>dynamically typed</strong>, which means you don't have to explicitly declare the data type of a variable. The interpreter infers the type at runtime based on the value assigned. You can even change the type of data a variable holds.</p>
                
                <div class="code-container">
                    <pre><code class="language-python">

                    # Assigning a string to a variable
full_name = "Alice Wonderland"

# Assigning an integer
age = 30

# The same variable can be reassigned to a different type
age = "thirty years old" 

# Multiple assignments in one line
x, y, z = "Orange", "Banana", "Cherry"
                    </code></pre>
                </div>
            </div>
        </section>

        <hr>

        <section id="operators">
            <h2>Python Basic Operators ⚙️</h2>
            <div class="section-content">
                <p>Operators are special symbols that perform computations. Let's explore the most common ones.</p>
                
                <h3>Arithmetic Operators:</h3>
                <p>Used to perform mathematical operations.</p>
                <div class="code-container">
                    <pre><code class="language-python">

                    x = 10
y = 3

print(x + y)   # Addition -> 13
print(x - y)   # Subtraction -> 7
print(x * y)   # Multiplication -> 30
print(x / y)   # Division -> 3.333...
print(x // y)  # Floor Division (discards the fractional part) -> 3
print(x % y)   # Modulus (returns the remainder) -> 1
print(x ** y)  # Exponentiation (x to the power of y) -> 1000
                    </code></pre>
                </div>

                <h3>Interactive Operator Panel:</h3>
                <p>Try it yourself! Enter two numbers and see the result of different operations.</p>
                <div class="interactive-panel">
                    <div class="inputs">
                        <input type="number" id="x" value="10">
                        <select id="operator">
                            <option value="+">+</option>
                            <option value="-">-</option>
                            <option value="*">*</option>
                            <option value="/">/</option>
                            <option value="//">//</option>
                            <option value="%">%</option>
                            <option value="**">**</option>
                        </select>
                        <input type="number" id="y" value="3">
                    </div>
                    <button id="calculate">Calculate</button>
                    <div class="output">
                        <p>Result: <span id="result">13</span></p>
                    </div>
                </div>
            </div>
        </section>

          <hr>

        <section id="blocks">
            <h2>Understanding Python Blocks 🧱</h2>
            <div class="section-content">
                <p>Unlike many other languages that use curly braces `{}` to define code blocks, Python uses <strong>indentation</strong>. A block of code begins with an indentation and ends with the first unindented line. The standard is to use <strong>four spaces</strong> per indentation level.</p>
                
                <h3>The Role of Indentation:</h3>
                <p>Indentation is not just for readability in Python; it's a strict syntax rule. Incorrect indentation will cause an <code>IndentationError</code>.</p>
                
                <div class="code-grid">
                    <div class="code-container">
                        <h4>✅ Correct Example:</h4>
                        <pre><code class="language-python">
is_raining = True
if is_raining:
    print("Don't forget an umbrella!")  # This is inside the 'if' block
    print("And wear your boots.")       # This is also inside the 'if' block

print("Have a nice day!") # This is outside the 'if' block
                        </code></pre>
                    </div>
                    <div class="code-container">
                        <h4>❌ Incorrect Example:</h4>
                        <pre><code class="language-python">
if True:
print("This will cause an error!") # Error: expected an indented block
                        </code></pre>
                    </div>
                </div>
            </div>
        </section>

        <hr>

        <section id="datatypes">
            <h2>Python Data Types 📊</h2>
            <div class="section-content">
                <p>Data types are classifications of data items. Python has several built-in types. You can check the type of any object using the <code>type()</code> function.</p>
                
                <div class="data-type-cards">
                    <div class="card">
                        <h3>Integer (`int`)</h3>
                        <p>Represents positive or negative whole numbers without a decimal point.</p>
                        <pre><code>a = 100</code></pre>
                    </div>
                    <div class="card">
                        <h3>Float (`float`)</h3>
                        <p>Represents numbers with a decimal point or in exponential form.</p>
                        <pre><code>b = 3.14</code></pre>
                    </div>
                    <div class="card">
                        <h3>String (`str`)</h3>
                        <p>An ordered sequence of characters, enclosed in single, double, or triple quotes.</p>
                        <pre><code>c = "Hello, World!"</code></pre>
                    </div>
                    <div class="card">
                        <h3>Boolean (`bool`)</h3>
                        <p>Represents one of two logical values: <code>True</code> or <code>False</code>.</p>
                        <pre><code>d = True</code></pre>
                    </div>
                </div>

                <h3>Other Important Data Types:</h3>
                <p>Python also has powerful collection data types:</p>
                <ul>
                    <li><strong>List (`list`):</strong> An ordered and mutable (changeable) collection. Example: `my_list = [1, "apple", 3.5]`</li>
                    <li><strong>Tuple (`tuple`):</strong> An ordered and immutable (unchangeable) collection. Example: `my_tuple = (1, "apple", 3.5)`</li>
                    <li><strong>Dictionary (`dict`):</strong> An unordered collection of key-value pairs. Example: `my_dict = {"name": "John", "age": 30}`</li>
                </ul>
            </div>
        </section>
    </main>

    <footer>
        <p>Next Steps: Dive into Control Flow, Functions, and more!</p>
        <div class="social-links">
            <a href="#">Twitter</a> | <a href="#">GitHub</a> | <a href="#">LinkedIn</a>
        </div>
        <p>&copy; 2025 PyLearn. Created with ❤️ in India.</p>
        <a href="#" class="back-to-top">▲</a>
    </footer>
    
    <script src="https://cdnjs.cloudflare.com/ajax/libs/prism/1.29.0/prism.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/prism/1.29.0/plugins/autoloader/prism-autoloader.min.js"></script>
    <script src="script.js"></script>
</body>
</html>


                    
