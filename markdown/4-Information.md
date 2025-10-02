## 4. Information theory

### 4.1 Entropy

<u>Definition</u>: Let $x,y \in \{0,1\}^n$. The Hamming distance between <u>x and y</u> is:

$$
d_H:\ \{0,1\}^n \times \{0,1\}^n \to \mathbb{N},
$$

$$
d_H(x,y) = \sum_{i=1}^n |x_i - y_i|
          = \bigl|\{\, i \in \{1,\dots,n\} \mid x_i \ne y_i \,\}\bigr|.
$$

*Entropy* is a core concept of **Information theory**; The average uncertainty in a source.

<u>Definition</u>: Let $t \in (0,1)$. The *binary entropy* of t is:
$$
h(t)= t\,\log_2\!\frac{1}{t} + (1-t)\,\log_2\!\frac{1}{1-t}
$$

<u>Definition</u>: Let X be a random variable whose values are 
$
\mathfrak{X} = \{X_1,...,X_n\}$ and $p_i = \mathbb{P}[X = X_i]  
\forall i = 1,...,n
$
is a probability distribution.  

The entropy of a random variable following a probability distribution P is equal to the entropy of P.

<u>Definition</u>: Similary, we can define the joint entropy of two (or more) random variables: $x \in \mathfrak{X}; y \in \mathfrak{Y}$:

$H(X,Y) := H\big((X \land Y)\big) = \sum_{(x,y) \in \mathfrak{X} \times \mathfrak{Y}} P[X = x, Y = y] \cdot \log \frac{1}{P[X = x, Y = y]}$

(We are saying that the entropy of X and Y are defined as the entropy of the couple (X,Y)).

<u>Definition</u>: The **INFORMATION CONTENT** or **SURPRISAL** of an event E is a function that grows with the unlirelihood of the event and is defined as:
$I[E] = -log_2\mathbb{P}[E] = log_2\frac{1}{\mathbb{P}[E]}$.

---

#### <u>Binary Encodings</u>

Let $\mathfrak{X}, |\mathfrak{X}| < \infty$ be an alphabet and let:

$M = \{\text{word of a language on } \mathfrak{X}\}$

$M^* = \{\text{sequences of words in } M\}$

$|M| < \infty, \; |M^*| = \infty, \; M^* = \bigcup_{i=1}^{\infty} M^i, 
\quad \text{where } M^i = \{\text{sequences of $i$ words in } M\}$

We denote a word as $m \in M$, and a sequence of words as $m \in M^*$.



<u>Definition</u>: A **variable length binary encoding** is an injective function  
$f : M \to \{0,1\}^*$ that assigns a binary string to each word in $M$.



<u>Definition</u>: We can extend this definition by juxtaposing several binary encodings and define the extension by concatenation $f^*$ of the variable length binary encoding $f$ as:  

$$
f^* : M^* \to \{0,1\}^*, \quad 
f^*(m) = f(m_1)\ldots f(m_n) \quad \text{if } m = (m_1, \ldots, m_n).
$$


→ Notice that $f^*$ can be non-injective.  
For example, let:  

$$
f(m_1) = 0, \quad f(m_2) = 1, \quad f(m_3) = 01.
$$  

Then  

$$
f^*(m = (m_1, m_2)) = 01 = f^*(m_3).
$$



<u>Definition</u>: A variable-length binary encoding $f : M \to \{0,1\}^*$ is **prefix-free**  
if $\forall m, m' \in M, \; m \neq m'$, it holds that:  

$$
f(m) \nless f(m'),
$$

where $x \nless y$ means *"x is not a prefix of y"*.

- We say that $x \prec y$ (*x is a prefix of y*) if: $\underline{x} = \underline{y}$ or $\exist \underline{z} \in \{0,1\}^*$ such that $\underline{x} = \underline{y}$.

<u>Definition</u> A binary encoding f is **U.D.** if its extension by concatenation $f^*$ is injective.


### 4.2 Mutual Information
<u>Definition</u>: Let X,Y be R.V. The **MUTUAL INFORMATION** of X and Y is defined as:

$$I(X,Y) = H(Y)-H(Y|X)$$

---

#### <u>Discrete Memoryless Channels (DMC)</u>

A Discrete Memoryless Channel (DMC) is a mathematical model of a communication channel.  
- *Discrete*: the input and output alphabets are finite sets.  
- *Memoryless*: the current output depends only on the current input, not on previous symbols.  
It is fully described by its transition probability matrix $P(y|x)$, which gives the probability of receiving output $y$ given input $x$.

---

#### <u>Differential Entropy and Channel Capacity</u>

For continuous random variables, we define **differential entropy** instead of discrete entropy.  
For a Gaussian random variable $X \sim \mathcal{N}(0, \sigma^2)$, the entropy is:

$$
h(X) = \tfrac{1}{2}\log_2(2\pi e \sigma^2).
$$

This leads to the definition of the **capacity** of a Gaussian channel with bandwidth $B$ and signal-to-noise ratio (SNR):

$$
C(B) = B \log_2(1 + \text{SNR}),
$$

known as the **Shannon-Hartley Theorem**, which follows from the Nyquist-Shannon sampling theorem.