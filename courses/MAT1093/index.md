---
layout: page
title: Precalculus
parent: Content by Course
nav_order: 1
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
# Precalculus Materials

- TOC
{:toc}

## Textbook

- [Topics in Precalculus](https://utsa.pressbooks.pub/precalculus/)

## The Unit Circle

<p align="center">
  <img src="/MathGym/assets/images/Unit Circle.jpg" alt="Unit Cricle" style="width:100%;">
</p>

## Trigonometric Identities

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

## Law of Sine and Cosines

Let $\alpha, \beta, \gamma$ be angles of a triangle with opposite corresponding side lengths of $a, b, c$ as show below.

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

## Polar Identities

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

## Exponential/Logarithmic Properties

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

---

This is an example of inline \\(\LaTeX\\). The following is Stokes' theorem in a
`displaymath` environment: \$$\int_{\partial \Omega} \omega = \int_{\Omega} d\omega\$$
