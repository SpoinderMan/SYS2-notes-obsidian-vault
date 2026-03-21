## $$F(s) = \int{f(s) \cdot e^{-st}}$$ 
## where $s = \sigma + j\omega$  

Laplace transform is an integral transform which simplifies convolution to multiplication and allows a [[Transfer Function]] to be expressed as a simple ratio ($G(s) = \dfrac {I(s)} {O(s)}$), where I and O are LTs of input and output respectively.

This is similar to a fourier transform, but laplace also covers the cases where system isnt in continuous steady oscillation, but has decay / boundless growth
Also for oscillatory systems, the output function is different for all varying starting cases. Laplace transform allows generalising a solution for any initial conditions.


## Inverse Laplace Transform : 
Formula : 
## $$f(t) = \dfrac{1}{2\pi j}\int_{\sigma - j\omega}^{\sigma + j\omega}{F(s)\cdot e^{-st}}$$
| **#**   | **$f(t)$**                           | **$F(s)=\mathcal{L}{f(t)}$**                                    |
| --- | -------------------------------- | ----------------------------------------------------------- |
| **1**   | **$1$**                              | **$\frac{1}{s}$**                                               |
| **2**   | **$e^{at}$**                         | **$\frac{1}{s-a}$**                                             |
| **3**   | **$t^n,; n\in\mathbb{N}$**           | **$\frac{n!}{s^{n+1}}$**                                        |
| **4**   | **$t^p,; p>-1$**                     | **$\frac{\Gamma(p+1)}{s^{p+1}}$**                               |
| **5**   | **$\sqrt{t}$**                       | **$\frac{\sqrt{\pi}}{2s^{3/2}}$**                               |
| **6**   | **$t^{n-\frac{1}{2}}$**              | **$\frac{1\cdot3\cdot5\cdots(2n-1)\sqrt{\pi}}{2^n s^{n+1/2}}$** |
| **7**   | **$\sin(at)$**                       | **$\frac{a}{s^2+a^2}$**                                         |
| **8**   | **$\cos(at)$**                       | **$\frac{s}{s^2+a^2}$**                                         |
| **9**   | **$t\sin(at)$**                      | **$\frac{2as}{(s^2+a^2)^2}$**                                   |
| **10**  | **$t\cos(at)$**                      | **$\frac{s^2-a^2}{(s^2+a^2)^2}$**                               |
| **11**  | **$\sin(at)-at\cos(at)$**            | **$\frac{2a^3}{(s^2+a^2)^2}$**                                  |
| **12**  | **$\sin(at)+at\cos(at)$**            | **$\frac{2as^2}{(s^2+a^2)^2}$**                                 |
| **13**  | **$\cos(at)-at\sin(at)$**            | **$\frac{s(s^2-a^2)}{(s^2+a^2)^2}$**                            |
| **14**  | **$\cos(at)+at\sin(at)$**            | **$\frac{s(s^2+3a^2)}{(s^2+a^2)^2}$**                           |
| **15**  | **$\sin(at+b)$**                     | **$\frac{s\sin b + a\cos b}{s^2+a^2}$**                         |
| **16**  | **$\cos(at+b)$**                     | **$\frac{s\cos b - a\sin b}{s^2+a^2}$**                         |
| **17**  | **$\sinh(at)$**                      | **$\frac{a}{s^2-a^2}$**                                         |
| **18**  | **$\cosh(at)$**                      | **$\frac{s}{s^2-a^2}$**                                         |
| **19**  | **$e^{at}\sin(bt)$**                 | **$\frac{b}{(s-a)^2+b^2}$**                                     |
| **20**  | **$e^{at}\cos(bt)$**                 | **$\frac{s-a}{(s-a)^2+b^2}$**                                   |
| **21**  | **$e^{at}\sinh(bt)$**                | **$\frac{b}{(s-a)^2-b^2}$**                                     |
| **22**  | **$e^{at}\cosh(bt)$**                | **$\frac{s-a}{(s-a)^2-b^2}$**                                   |
| **23**  | **$t^n e^{at}$**                     | **$\frac{n!}{(s-a)^{n+1}}$**                                    |
| **24**  | **$f(ct)$**                          | **$\frac{1}{c}F\left(\frac{s}{c}\right)$**                      |
| **25**  | **$u(t-c)$**                         | **$\frac{e^{-cs}}{s}$**                                         |
| **26**  | **$\delta(t-c)$**                    | **$e^{-cs}$**                                                   |
| **27**  | **$u(t-c)f(t-c)$**                   | **$e^{-cs}F(s)$**                                               |
| **28**  | **$u(t-c)g(t)$**                     | **$e^{-cs}\mathcal{L}{g(t+c)}$**                                |
| **29**  | **$e^{ct}f(t)$**                     | **$F(s-c)$**                                                    |
| **30**  | **$t^n f(t)$**                       | **$(-1)^n F^{(n)}(s)$**                                         |
| **31**  | **$\frac{1}{t}f(t)$**                | **$\int_s^\infty F(u),du$**                                     |
| **32**  | **$\int_0^t f(v),dv$**               | **$\frac{F(s)}{s}$**                                            |
| **33**  | **$\int_0^t f(t-\tau)g(\tau)d\tau$** | **$F(s)G(s)$**                                                  |
| **34**  | **$f(t+T)=f(t)$**                    | **$\frac{\int_0^T e^{-st}f(t),dt}{1-e^{-sT}}$**                 |
| **35**  | **$f'(t)$**                          | **$sF(s)-f(0)$**                                                |
| **36**  | **$f''(t)$**                         | **$s^2F(s)-sf(0)-f'(0)$**                                       |
| **37**  | **$f^{(n)}(t)$**                     | **$s^nF(s)-s^{n-1}f(0)-\cdots-f^{(n-1)}(0)$**                   |
