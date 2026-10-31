---
layout: page
title: Calculus I
parent: Content by Course
nav_order: 4
katex: true
---

{% if page.katex %}

<!-- CSS -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@latest/dist/katex.min.css"/>

<!-- JavaScript -->
<script defer src="https://cdn.jsdelivr.net/npm/katex@latest/dist/katex.min.js"></script>
<script defer src="https://cdn.jsdelivr.net/npm/katex@latest/dist/contrib/auto-render.min.js"
  onload="renderMathInElement(document.body,{
    delimiters: [
      { left: '$$',  right: '$$',  display: true  },
      { left: '$',   right: '$',   display: false },
      { left: '\\[', right: '\\]', display: true  },
      { left: '\\(', right: '\\)', display: false }
  ]});">
</script>

{% endif %}

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

# Textbook

- [Calculus - Volume 1](https://openstax.org/details/books/calculus-volume-1?Book%20details)

# Limits

## Notation

<p align="center">
  <table>
  <tr>
    <th>Left Limit</th>
    <th>General Limit</th>
    <th>Right Limit</th>
  </tr>
  <tr>
    <td>
The limit of $f(x)$ as $x$ approaches $a$ from the left is written as
$$ \lim_{x \to a^-} f(x) $$
</td>
    <td>
The limit of $f(x)$ as $x$ approaches $a$ is written as
$$ \lim_{x \to a} f(x) $$
</td>
    <td>
The limit of $f(x)$ as $x$ approaches $a$ from the right is written as
$$ \lim_{x \to a^+} f(x) $$
</td>
  </tr>
  </table>
</p>

## Limit Laws

<p align="center">
  <table>
  <tr>
    <th>Basic Limit Results</th>
  </tr>
  <tr>
    <td>
For any real number $a$ and any constant $c$,
$$ \lim_{x \to a} x = a $$
and
$$ \lim_{x \to a} c = c $$
</td>
  </tr>
  </table>
  <table>
  <tr>
    <th>Limit Laws</th>
  </tr>
  <tr>
    <td>
Let $f(x)$ and $g(x)$ be defined for all $x \neq a$ over some open interval containing $a$. Assume that $L$ and $M$ are real numbers such that $\underset{x \to a}\lim f(x) = L$ and $\underset{x \to a}\lim g(x) = M$. Let $c$ be a constant. Then, each of the following statements holds:
</td>
  </tr>
  <tr>
    <td>
Sum/Difference law:
$$ \lim_{x \to a} \left( f(x) \pm g(x)\right) = \lim_{x \to a} f(x) \pm \lim_{x \to a} g(x) = L \pm M $$
</td>
  </tr>
  <tr>
    <td>
Constant multiple law:
$$ \lim_{x \to a} \left( f(x) \cdot g(x)\right) = \lim_{x \to a} f(x) \cdot \lim_{x \to a} g(x) = L \cdot M $$
</td>
  </tr>
  <tr>
    <td>
Quotient law:
$$ \lim_{x \to a} \left( f(x) / g(x)\right) = \lim_{x \to a} f(x) / \lim_{x \to a} g(x) = \frac{L}{M} \text{ for $M \neq 0$} $$
</td>
  </tr>
  </table>
</p>

## Continuity

### Continuous functions

<p align="center">
  <table>
  <tr>
    <th>Continuity</th>
  </tr>
  <tr>
    <td>
A Function $f(x)$ is continuous at a point $a$ if and only if the following three conditions are satisfied:
<ol>
  <li>$f(a)$ is defined</li>
  <li>$\underset{x \to a}\lim f(x)$ exists</li>
  <li>$\underset{x \to a}\lim f(x) = f(a)$</li>
</ol>
A function is discontinuous at a point a if it fails to be continuous at $a$.
</td>
  </tr>
  </table>
</p>

### Discontinuities

<p align="center">
  <table>
  <tr>
    <th>Removable Discontinuity</th>
    <th>Jump Discontinuity</th>
    <th>Infinite Discontinuity</th>
  </tr>
  <tr>
    <td>
  <img src="/MathGym/assets/images/Removable.jpg" alt="Removable Discontinuity" style="width:100%;">
</td>
    <td>
  <img src="/MathGym/assets/images/Jump.jpg" alt="Jump Discontinuity" style="width:100%;">
</td>
    <td>
  <img src="/MathGym/assets/images/Infinite.jpg" alt="Infinite Discontinuity" style="width:100%;">
</td>
  </tr>
  </table>
</p>

# Derivatives

## Slope

<p align="center">
  <table>
  <tr>
    <th>Slope of the Secant Line</th>
    <th>Slope of the Tangent Line</th>
  </tr>
  <tr>
    <td>
$$ m_{\text{sec}} = \dfrac{f(x) - f(a)}{x - a} $$
</td>
    <td>
$$ m_{\text{tan}} = \lim_{x \to a} \dfrac{f(x) - f(a)}{x - a} $$
or
$$ m_{\text{tan}} = \lim_{h \to 0} \dfrac{f(a + h) - f(a)}{h} $$
</td>
  </tr>
  </table>
</p>

## Limit Definition

<p align="center">
  <table>
  <tr>
    <th>The Derivative at a Point</th>
  </tr>
  <tr>
    <td>
$$ f'(a) = \lim_{x \to a} \dfrac{f(x) - f(a)}{x - a} $$
or
$$ f'(a) = \lim_{h \to 0} \dfrac{f(a + h) - f(a)}{h} $$
</td>
  </tr>
  </table>
  <table>
  <tr>
    <th>The Derivative as a Function</th>
  </tr>
  <tr>
    <td>
$$ f'(x) = \lim_{h \to 0} \dfrac{f(x + h) - f(x)}{h} $$
</td>
  </tr>
  </table>
</p>

## Notations

<p align="center">
  <table>
  <tr>
    <th>Newton</th>
    <th>Leibniz</th>
  </tr>
  <tr>
    <td>
$$ f'(x) \quad \text{or} \quad \left( f(x) \right)' $$
</td>
    <td>
$$ \frac{df}{dx}(x) \quad \text{or} \quad \frac{d}{dx}f(x) $$
</td>
  </tr>
  </table>
</p>

## Derivative Rules

<p align="center">
  <table>
  <tr>
    <th>Constant Rule</th>
  </tr>
  <tr>
    <td>
$$ \frac{d}{dx} c = 0 $$
</td>
  </tr>
  </table>
<!-- BREAK -->
  <table>
  <tr>
    <th>Power Rule</th>
  </tr>
  <tr>
    <td>
$$ \frac{d}{dx} x^n = nx^{n - 1} $$
</td>
  </tr>
  </table>
<!-- BREAK -->
  <table>
  <tr>
    <th>Sum/Difference Rule</th>
  </tr>
  <tr>
    <td>
$$ \frac{d}{dx} \left( f(x) \pm g(x) \right) = \frac{d}{dx} \left( f(x) \right) \pm \frac{d}{dx} \left( g(x) \right) $$
</td>
  </tr>
  </table>
<!-- BREAK -->
  <table>
  <tr>
    <th>Constant Multiple Rule</th>
  </tr>
  <tr>
    <td>
$$ \frac{d}{dx} \left( kf(x) \right) = k \frac{d}{dx} \left( f(x) \right) $$
</td>
  </tr>
  </table>
<!-- BREAK -->
  <table>
  <tr>
    <th>Eponential Rule</th>
  </tr>
  <tr>
    <td>
$$ \frac{d}{dx} \left( a^x \right) = \ln(a) a^x $$
Special Case:
$$ \frac{d}{dx} \left( e^x \right) = e^x $$
</td>
  </tr>
  </table>
<!-- BREAK -->
  <table>
  <tr>
    <th>Logarithm Rule</th>
  </tr>
  <tr>
    <td>
$$ \frac{d}{dx} \left( \log_a x \right) = \frac{1}{\ln(a)x} $$
Special Case:
$$ \frac{d}{dx} \left( \ln x \right) = \frac{1}{x} $$
</td>
  </tr>
  </table>
<!-- BREAK -->
  <table>
  <tr>
    <th>Product Rule</th>
  </tr>
  <tr>
    <td>
$$ \frac{d}{dx} \left( f(x) g(x) \right) = f'(x) g(x) + g'(x) f(x) $$
</td>
  </tr>
  </table>
<!-- BREAK -->
  <table>
  <tr>
    <th>Quotient Rule</th>
  </tr>
  <tr>
    <td>
$$ \frac{d}{dx} \left( \frac{f(x)}{g(x)} \right) = \frac{f'(x) g(x) - g'(x) f(x)}{\left( g(x) \right)^2} $$
</td>
  </tr>
  </table>
</p>

## Trigonometric Derivatives

<p align="center">
  <table>
  <tr>
    <th>Standard Functions</th>
  </tr>
  <tr>
    <td>
$$ \frac{d}{dx} \sin x = \cos x $$
$$ \frac{d}{dx} \cos x = -\sin x $$
$$ \frac{d}{dx} \tan x = \sec^2 x $$
$$ \frac{d}{dx} \sec x = \sec x \tan x $$
$$ \frac{d}{dx} \csc x = -\csc x \cot x $$
$$ \frac{d}{dx} \cot x = \csc^2 x $$
</td>
  </tr>
  </table>
<!-- BREAK -->
  <table>
  <tr>
    <th>Inverse Functions</th>
  </tr>
  <tr>
    <td>
$$ \frac{d}{dx} \sin^{-1} x = \frac{1}{\sqrt{1 - x^2}} $$
$$ \frac{d}{dx} \cos^{-1} x = -\frac{1}{\sqrt{1 - x^2}} $$
$$ \frac{d}{dx} \tan^{-1} x = \frac{1}{1 + x^2} $$
$$ \frac{d}{dx} \sec^{-1} x = \frac{1}{|x|\sqrt{1 - x^2}} $$
$$ \frac{d}{dx} \csc^{-1} x = -\frac{1}{|x|\sqrt{1 - x^2}}  $$
$$ \frac{d}{dx} \cot^{-1} x = -\frac{1}{1 + x^2} $$
</td>
  </tr>
  </table>
</p>

## The Chain Rule

<p align="center">
  <table>
  <tr>
    <td>
$$ \frac{d}{dx} \left( f\left(g(x)\right) \right) = f'\left(g(x)\right)g'(x) $$
</td>
  </tr>
  </table>
</p>

## Inverse Functions

<p align="center">
  <table>
  <tr>
    <td>
Let $(a,b)$ be a point, where $f(a) = b$ and $f^{-1}(b) = a$, then
$$ \left( f^{-1} \right)'(b) = \frac{1}{f'(a)} $$
</td>
  </tr>
  </table>
</p>