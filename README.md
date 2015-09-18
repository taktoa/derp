# Derp: derivative parsing for Haskell

A parser based on derivatives of parser combinators (Might and Darais).

Our paper on Arxiv details the theory of parsing with derivatives:
[arxiv](http://arxiv.org/abs/1010.5023).

This implementation uses my latest work on the theory that brings the $O(n*|G|^2)$
complexity bound to $O(n)$ for parsing most not-painfully-ambiguous grammars, where
$|G|$ is the size of the initial grammar and $n$ is the size of the input.

These bounds are based off of observation and intuition; they are not proven yet.

This implementation will not terminate if the resulting parse forest is
infinite. We know how to extend the implementation to work for infinite parse
forests with little effort. If you're interested, send me an email.
