# Indicator Function for Palindromic Numbers

As demonstrated in the research paper, below are two function that can indicate if a integer $n$ is a palindromic number.

$$D_1(n) = \left\lfloor
\frac{1}{N(n)} \sum_{i=0}^{N(n)-1}
\left\lfloor
\frac{\left\lfloor 10\left(\frac{n}{10^{i+1}} - \left\lfloor \frac{n}{10^{i+1}} \right\rfloor\right) \right\rfloor\ + \epsilon}
{\left\lfloor 10\left(\frac{n}{10^{N(n)-i}} - \left\lfloor \frac{n}{10^{N(n)-i}} \right\rfloor\right) \right\rfloor + \epsilon}
\right\rfloor
\cdot
\left\lfloor
\frac{\left\lfloor 10\left(\frac{n}{10^{N(n)-i}} - \left\lfloor \frac{n}{10^{N(n)-i}} \right\rfloor\right) \right\rfloor + \epsilon}
{\left\lfloor 10\left(\frac{n}{10^{i+1}} - \left\lfloor \frac{n}{10^{i+1}} \right\rfloor\right) \right\rfloor + \epsilon}
\right\rfloor
\right\rfloor$$

$$D_2(n) = \prod_{i=0}^{N(n)-1}
\left\lfloor
\frac{\left\lfloor 10\left(\frac{n}{10^{i+1}} - \left\lfloor \frac{n}{10^{i+1}} \right\rfloor\right) \right\rfloor\ + \epsilon}
{\left\lfloor 10\left(\frac{n}{10^{N(n)-i}} - \left\lfloor \frac{n}{10^{N(n)-i}} \right\rfloor\right) \right\rfloor + \epsilon}
\right\rfloor
\cdot
\left\lfloor
\frac{\left\lfloor 10\left(\frac{n}{10^{N(n)-i}} - \left\lfloor \frac{n}{10^{N(n)-i}} \right\rfloor\right) \right\rfloor + \epsilon}
{\left\lfloor 10\left(\frac{n}{10^{i+1}} - \left\lfloor \frac{n}{10^{i+1}} \right\rfloor\right) \right\rfloor + \epsilon}
\right\rfloor.$$

Both functions rerturn $1$ when $n$ is a palindromic number and $0$ otherwise.
