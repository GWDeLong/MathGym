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

# Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}

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
  <li>$\underset{x \to a} f(x)$ exists</li>
  <li>$\underset{x \to a} f(x) = f(a)$</li>
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
$$ m_{\text{sec} = \dfrac{f(x) - f(a)}{x - a} $$
</td>
    <td>
$$ m_{\text{tan} = \lim_{x \to a} \dfrac{f(x) - f(a)}{x - a} $$
or
$$ m_{\text{tan} = \lim_{h \to 0} \dfrac{f(a + h) - f(a)}{h} $$
</td>
  </tr>
  </table>
</p>

## The Derivative

### Limit Definition

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

### Notations

<p align="center">
  <table>
  <tr>
    <th>Newton</th>
    <th>Leibniz</th>
  </tr>
  <tr>
    <td>
$$ f'(x) \text{ or } \left( f(x) \right)' $$
</td>
    <td>
$$ \frac{df}{dx}(x) \text{ or } \frac{d}{dx}f(x) $$
</td>
  </tr>
  </table>
</p>

### Derivative Rules

<p align="center">
  <table>
  <tr>
    <th>Constant Rule</th>
  </tr>
  <tr>
    <td>
$$  $$
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







# The Unit Circle

<p align="center">
  <img src="/MathGym/assets/images/Unit Circle.jpg" alt="Unit Circle" style="width:100%;">
</p>

# Trigonometric Identities

<p align="center">
  <table>
  <tr>
    <th>Reciprocal Identities</th>
    <th>Quotient Identities</th>
  </tr>
  <tr>
    <td>
$$ \sin\theta = \dfrac{1}{\csc\theta} \quad \cos\theta = \dfrac{1}{\sec\theta} \quad \tan\theta = \dfrac{1}{\cot\theta}$$
$$ \csc\theta = \dfrac{1}{\sin \theta} \quad \sec\theta = \dfrac{1}{\cos\theta} \quad \cot\theta = \dfrac{1}{\tan\theta} $$
</td>
    <td>
$$ \tan\theta = \dfrac{\sin\theta}{\cos\theta} \quad \cot\theta = \dfrac{\cos\theta}{\sin\theta} $$
</td>
  </tr>
  </table>
<!-- BREAK -->
  <table>
  <tr>
    <th>Pythagorean Identities</th>
  </tr>
  <tr>
    <td>
$$ \sin^2\theta + \cos^2\theta = 1 \qquad \tan^2\theta + 1 = \sec^2\theta \qquad \cot^2\theta + 1 = \csc^2\theta $$
</td>
  </tr>
  </table>
<!-- BREAK -->
  <table>
  <tr>
    <th>Cofunction Identities</th>
    <th>Even-Odd Identities</th>
  </tr>
  <tr>
    <td>
$$ \sin\theta = \cos\left( \frac{\pi}{2} - \theta \right) \quad \cos\theta = \sin\left( \frac{\pi}{2} - \theta \right)$$
$$ \csc\theta = \sec\left( \frac{\pi}{2} - \theta \right) \quad \sec\theta = \csc\left( \frac{\pi}{2} - \theta \right)$$
$$ \tan\theta = \cot\left( \frac{\pi}{2} - \theta \right) \quad \cot\theta = \tan\left( \frac{\pi}{2} - \theta \right)$$
</td>
    <td>
$$ \sin(-\theta) = -\sin\theta \quad \csc(-\theta) = -\csc\theta $$
$$ \cos(-\theta) = \cos\theta \quad \sec(-\theta) = \sec\theta $$
$$ \tan(-\theta) = -\tan\theta \quad \cot(-\theta) = -\cot\theta $$
</td>
  </tr>
</table>
<!-- BREAK -->
  <table>
  <tr>
    <th>Sum of Angles Identities</th>
    <th>Difference of Angles Identities</th>
  </tr>
  <tr>
    <td>
$$ \sin\left( A + B \right) = \sin A \cdot \cos B + \cos A \cdot \sin B $$
$$ \cos\left( A + B \right) = \cos A \cdot \cos B - \sin A \cdot \sin B $$
$$ \tan\left( A + B \right) = \dfrac{\tan A + \tan B}{1 - \tan A \cdot \tan B}
$$
</td>
    <td>
$$ \sin\left( A - B \right) = \sin A \cdot \cos B - \cos A \cdot \sin B $$
$$ \cos\left( A - B \right) = \cos A \cdot \cos B + \sin A \cdot \sin B $$
$$ \tan\left( A - B \right) = \dfrac{\tan A - \tan B}{1 + \tan A \cdot \tan B}
$$
</td>
  </tr>
</table>
<!-- BREAK -->
  <table>
  <tr>
    <th>Double-Angle Identities</th>
  </tr>
  <tr>
    <td>
$$ \cos 2\theta = \cos^2\theta - \sin^2\theta $$
$$ \sin 2\theta = 2\sin\theta \cdot \cos\theta \qquad \cos 2\theta = 1 - 2\sin^2\theta \quad \tan 2\theta = \dfrac{2\tan \theta}{1 - \tan^2 \theta} $$
$$ \cos 2\theta = 2\cos^2\theta - 1 $$
</td>
  </tr>
  </table>
<!-- BREAK -->
  <table>
  <tr>
    <th>Half-Angle Identities</th>
  </tr>
  <tr>
    <td>
$$ \sin \frac{\theta}{2} = \pm \sqrt{\frac{1 - \cos \theta}{2}} \quad
\cos \frac{\theta}{2} = \pm \sqrt{\frac{1 + \cos \theta}{2}} $$
$$ \tan \frac{\theta}{2} = \pm \sqrt{\frac{1 - \cos \theta}{1 + \cos \theta}} \quad
\tan \frac{\theta}{2} = \frac{1 - \cos \theta}{\sin \theta} \quad
\tan \frac{\theta}{2} = \frac{\sin \theta}{1 + \cos \theta} $$
</td>
  </tr>
  </table>
<!-- BREAK -->
  <table>
  <tr>
    <th>Power-Reducing Identities</th>
  </tr>
  <tr>
    <td>
$$ \sin^2\theta = \frac{1 - \cos 2\theta}{2} \qquad \cos^2\theta = \frac{1 + \cos 2\theta}{2} \qquad \tan^2\theta = \frac{1 - \cos 2\theta}{1 + \cos 2\theta} $$
</td>
  </tr>
  </table>
<!-- BREAK -->
  <table>
  <tr>
    <th>Product-to-Sum Identities</th>
    <th>Sum-to-Product Identities</th>
  </tr>
  <tr>
    <td>
$$ \sin A \cdot \sin B = \frac{1}{2}\left[ \cos(A - B) - \cos(A + B) \right] $$
$$ \cos A \cdot \cos B = \frac{1}{2}\left[ \cos(A - B) + \cos(A + B) \right]  $$
$$ \sin A \cdot \cos B = \frac{1}{2}\left[ \sin(A + B) + \sin(A - B) \right]  $$
$$ \cos A \cdot \sin B = \frac{1}{2}\left[ \sin(A + B) - \sin(A - B) \right]  $$
</td>
    <td>
$$ \sin A + \sin B = 2\sin\left( \frac{A + B}{2} \right) \cdot \cos\left( \frac{A - B}{2} \right) $$
$$ \cos A + \cos B = 2\cos\left( \frac{A + B}{2} \right) \cdot \cos\left( \frac{A - B}{2} \right) $$
$$ \sin A - \sin B = 2\cos\left( \frac{A + B}{2} \right) \cdot \sin\left( \frac{A - B}{2} \right) $$
$$ \cos A - \cos B = -2\sin\left( \frac{A + B}{2} \right) \cdot \sin\left( \frac{A - B}{2} \right) $$
</td>
  </tr>
</table>
</p>

# Law of Sine and Cosines

Let $\alpha, \beta, \gamma$ be angles of a triangle with opposite corresponding side lengths of $a, b, c$ as shown below.

<p align="center">
  <img src="/MathGym/assets/images/Scalene Triangle.jpg" alt="Scalene Triangle" style="width:75%;">
</p>

The following laws are true.

<p align="center">
  <table>
  <tr>
    <th>Law of Sines</th>
  </tr>
  <tr>
    <td>
$$ \frac{\sin \alpha}{a} = \frac{\sin \beta}{b} = \frac{\sin \gamma}{c}. $$
</td>
  </tr>
  </table>
<!-- BREAK -->
  <table>
  <tr>
    <th>Law of Cosines</th>
  </tr>
  <tr>
    <td>
$$ a^2 = b^2 + c^2 - 2bc \cos \alpha $$
$$ b^2 = a^2 + c^2 - 2ac \cos \beta $$
$$ c^2 = a^2 + b^2 - 2ab \cos \gamma $$
</td>
  </tr>
  </table>
</p>

# Polar Identities

<p align="center">
  <table>
  <tr>
    <th>Polar to Rectangular Coordinates</th>
    <th>Rectangular to Polar Coordinates</th>
  </tr>
  <tr>
    <td>
$$ x = r \cos \theta $$
$$ y = r \sin \theta $$
</td>
    <td>
$$ r^2 = x^2 + y^2 $$
$$ \tan \theta = \frac{y}{x} $$
</td>
  </tr>
</table>
</p>

# Exponential/Logarithmic Properties

<p align="center">
  <table>
  <tr>
    <th>Exponential Rules</th>
	<th>Logarithmic Rules</th>
  </tr>
  <tr>
    <td>
Product Rule
$$ x^n\cdot x^m = x^{n + m} $$
Quotient Rule
$$ \frac{x^n}{x^m} = x^{n - m} $$
Power Rule
$$ \left( x^n \right)^m = x^{n\cdot m} $$
</td>
    <td>
Product Rule
$$ \log(AB) = \log(A) + \log(B) $$
Quotient Rule
$$ \log\left(\frac{A}{B}\right) = \log(A) - \log(B) $$
Power Rule
$$ \log\left( A^B \right) = B\log(A)$$
</td>
  </tr>
</table>
</p>
