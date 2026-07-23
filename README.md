# Indicator Function for Palindromic Numbers

As demonstrated in the research paper, below are two function that can indicate if a integer $n$ is a palindromic number.

$$D_1(n) = \left\lfloor \frac{1}{\left\lfloor \log(n)+1 \right\rfloor}  \sum_{k=1}^{\left\lfloor \log(n)+1 \right\rfloor}  \left\lfloor \frac{\left\lfloor 10 \bigg (\frac{n}{10^k} - \left\lfloor \frac{n}{10^k} \right\rfloor \bigg) + 1 \right\rfloor
}{\left\lfloor 10 \bigg (\frac{n}{10^{\left\lfloor \log(n)+1 \right\rfloor}} - \left\lfloor \frac{n}{10^{\left\lfloor \log(n)+1 \right\rfloor}} \right\rfloor \bigg) + 1 \right\rfloor}  \right\rfloor  \left\lfloor \frac{\left\lfloor 10 \bigg (\frac{n}{10^{\left\lfloor \log(n)+1 \right\rfloor}} - \left\lfloor \frac{n}{10^{\left\lfloor \log(n)+1 \right\rfloor}} \right\rfloor \bigg) + 1 \right\rfloor}{\left\lfloor 10 \bigg (\frac{n}{10^k} - \left\lfloor \frac{n}{10^k} \right\rfloor \bigg) + 1 \right\rfloor
} \right\rfloor  \right\rfloor$$

$$D_2(n) = \prod_{k=1}^{\left\lfloor \log(n)+1 \right\rfloor} \left\lfloor \frac{\left\lfloor 10 \bigg (\frac{n}{10^k} - \left\lfloor \frac{n}{10^k} \right\rfloor \bigg) + 1 \right\rfloor
}{\left\lfloor 10 \bigg (\frac{n}{10^{\left\lfloor \log(n)+1 \right\rfloor}} - \left\lfloor \frac{n}{10^{\left\lfloor \log(n)+1 \right\rfloor}} \right\rfloor \bigg) + 1 \right\rfloor}  \right\rfloor  \left\lfloor \frac{\left\lfloor 10 \bigg (\frac{n}{10^{\left\lfloor \log(n)+1 \right\rfloor}} - \left\lfloor \frac{n}{10^{\left\lfloor \log(n)+1 \right\rfloor}} \right\rfloor \bigg) + 1 \right\rfloor}{\left\lfloor 10 \bigg (\frac{n}{10^k} - \left\lfloor \frac{n}{10^k} \right\rfloor \bigg) + 1 \right\rfloor
} \right\rfloor.$$


With $D_1(n) = D_2(n) = \left\{ \begin{array}{cl} 1 & \ \text{si n est un palindrome} \\ 0 & \ \text{sinon} \end{array} \right$
