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

                    
