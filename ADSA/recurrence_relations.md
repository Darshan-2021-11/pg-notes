# T(n) = 3T(sq(n)) + 1
Let n = 2^m
T(2^m) = 3T(2^(m/2)) + 1
Let T(2^m) = S(m)
S(m) = 3S(m/2) + 1
Applying Master theorem:
S(m) = Theta(m ^ (log2(3)))
T(2^m) = Theta(m * log2(3))
T(n) = Theta(log2(n) * log2(3))

# T(n) = T(sq(n)) + n^2
Let n = 2^m
T(2^m) = T(2^(m/2)) + 2^(2m)
Let T(2^m) = S(m)
S(m) = S(m/2) + 2^(2m)
Applying Master theorem:
S(m) = Theta(2^(2m))
T(2^m) = Theta(2^(2m))
T(n) = Theta(2^(2log2(n)))
T(n) = Theta(2^(log2(n^2)))
T(n) = Theta(n^2)

# Recurrence relation involving square roots
n^(1/(2^k)) = 2
(1/(2^k)) * log2n = 1
log2n = 2^k
k = log2log2n
So,
T(n) = 1 + 2^1(1) + 2^2(1) + ... + 2^log2log2n(1)
T(n) = log2n
