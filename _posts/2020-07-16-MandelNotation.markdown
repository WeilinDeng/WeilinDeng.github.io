---
layout: post
title: Mandel's notation
date: 2020-07-16 18:00
description: Tensor representations
comments: true
---
$$
\def\bs#1{\boldsymbol #1}
\def\hbs#1{\hat{\boldsymbol {#1}}}
\def\ul#1{\underline{\underline{#1}}}
\newcommand{\pd}[2]{\frac{\partial #1}{\partial #2}}
$$

Mandel's notation represents symmetric, second rank tensors as column vectors, and fourth rank tensors with minor symmetries as matrices. This representation is defined below.

### Mandel notation in 3D
In this section, the notation is introduced for tensors of the three dimensional space.

#### Second order, symmetric tensors
Let $\bs{\varepsilon}$ be a second rank, symmetric tensor,

$$
\begin{equation}
  \varepsilon_{ij} = \epsilon_{ji}
  \label{eq:varepsilon}
\end{equation}
$$

Its Mandel representation $$[\bs{\varepsilon}]$$ (as a column-vector) is defined as follows:

$$
\begin{equation}
  [\bs{\varepsilon}] = [\varepsilon_{11}, \varepsilon_{22}, \varepsilon_{33}, \sqrt{2}\varepsilon_{23}, \sqrt{2}\varepsilon_{31}, \sqrt{2}\varepsilon_{12}]^{\rm T},
\end{equation}
$$

where the cross-component $\varepsilon_{ij}$ ($i \neq j$) appears at the $3+k^{\rm th}$ line, with $k \neq i \neq j$. The $\sqrt{2}$ prefactors ensure that the standard scalar product of column vectors coincides with the double contraction of tensors. Indeed

$$
\begin{equation}
\begin{aligned}
  \boldsymbol\sigma:\boldsymbol\varepsilon&=\sigma_{ij}\varepsilon_{ij} \\
  &=\sigma_{11}\varepsilon_{11}+\sigma_{22}\varepsilon_{22}+\sigma_{33}\varepsilon_{33}+2\sigma_{23}\varepsilon_{23}+2\sigma_{31}\varepsilon_{31}+2\sigma_{12}\varepsilon_{12} \\
  &=[\boldsymbol\sigma]^\mathrm{T}\cdot[\boldsymbol\varepsilon].
\end{aligned}
\end{equation}
$$


#### Fourth order tensors with minor symmetries
Let $\bs{C}$  be a fourth order tensor with minor symmetries,

$$
\begin{equation}
  C_{ijkl}=C_{jikl}=C_{ijlk}.
\end{equation}
$$

Its Mandel representation $[\bs{C}]$ (as a square matrix) is defined as follows:

$$
\begin{equation}
  [\mathbf C] =
  \begin{bmatrix}
    C_{1111} & C_{1122} & C_{1133} & \sqrt{2}C_{1123} & \sqrt{2}C_{1131} & \sqrt{2}C_{1112}\\
    C_{2211} & C_{2222} & C_{2233} & \sqrt{2}C_{2223} & \sqrt{2}C_{2231} & \sqrt{2}C_{2212}\\
    C_{3311} & C_{3322} & C_{3333} & \sqrt{2}C_{3323} & \sqrt{2}C_{3331} & \sqrt{2}C_{3312}\\
    \sqrt{2}C_{2311} & \sqrt{2}C_{2322} & \sqrt{2}C_{2333} & 2C_{2323} & 2C_{2331} & 2C_{2312}\\
    \sqrt{2}C_{3111} & \sqrt{2}C_{3122} & \sqrt{2}C_{3133} & 2C_{3123} & 2C_{3131} & 2C_{3112}\\
    \sqrt{2}C_{1211} & \sqrt{2}C_{1222} & \sqrt{2}C_{1233} & 2C_{1223} & 2C_{1231} & 2C_{1212}
  \end{bmatrix},
\end{equation}
$$

where the numbering of the cross-components $C_{ijkl}$ with $i \neq j$ or $k \neq l$ is consistent with the numbering of cross-components of second order tensors. Again, the $\sqrt{2}$ and 2 prefactors ensure that matrix-matrix and matrix-vector products coincide with the double contraction of tensors.

More precisely, the Mandel representation of the second order tensor $\bs{\sigma} = \bs{C}:\bs{\varepsilon}$ is the column vector

$$
\begin{equation}
[\boldsymbol\sigma]=[\mathbf C:\boldsymbol\varepsilon]=C_{ijkl}\varepsilon_{kl}=[\mathbf C]\cdot[\boldsymbol\varepsilon].
\end{equation}
$$

Likewise, if $\bs{S}$ is another fourth order tensor with minor symmetries, then

$$
\begin{equation}
[\bs{C}:\bs{s}] = [\bs{C}]\cdot[\bs{s}],
\end{equation}
$$

where it is recalled that the $(i, j, k, l)$ component of $\bs{C}:\bs{s}$ is $C_{ijmn}S_{mnkl}$. It results from the above formula that the Mandel representation of the inverse of a fourth order tensor is the inverse of the Mandel representation of this tensor

$$
\begin{equation}
  [\bs{C}^{-1}] = [\bs{C}]^{−1}.
\end{equation}
$$

Finally, it is readily verified that the Mandel representation of the transpose is the transpose of the Mandel representation

$$
\begin{equation}
  [\bs{C}^{\rm T}] = [\bs{C}]^{\rm T}.
\end{equation}
$$



### Mandel's notation in 2D
The above formulas are readily extended to two dimensions, so that we only recall the matrix representation of second order, symmetric tensors and fourth order tensors with minor symmetries. The properties of these matrix representations are unchanged.

#### Second order, symmetric tensors
The Mandel representation $[\bs{\varepsilon}]$ (as a column-vector) of any second order, symmetric tensor $\bs{\varepsilon}$ is defined as follows

$$
\begin{equation}
  [\bs{\varepsilon}] = [\varepsilon_{11},\varepsilon_{22},\sqrt{2}\varepsilon_{12}]^{\rm T}.
\end{equation}
$$

#### Fourth order tensors with minor symmetries
The Mandel representation $[\bs{C}]$ (as a square matrix) of any fourth order tensor $\bs{C}$ with minor symmetries is defined as follows:

$$
\begin{equation}
  [\mathbf C] =
  \begin{bmatrix}
    C_{1111} & C_{1122} & \sqrt{2}C_{1112}\\
    C_{2211} & C_{2222} & \sqrt{2}C_{2212}\\
    \sqrt{2}C_{1211} & \sqrt{2}C_{1222} & 2C_{1212}
  \end{bmatrix}.
\end{equation}
$$
