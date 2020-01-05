In the Decryption_MCMC notebook, we will decrypt a passage from the Great Gatsby that has been encrypted by remapping each symbol to a (usually) different one. For example, a text like 'my father...' might be encypted by 'lq!bhuwbt'. We assume that the mapping between symbols is one-to-one. The file symbols.txt gives the list of symbols, one per line. The file message.txt gives the encrypted message.

Decoding the message by brute force is impossible, since there are 53 symbols and thus 53! possible permutations to try. Instead we will set up a Markov chain Monte Carlo sampler tofind modes in the space of permutations.

We learn the transition statistics of letters and punctuation in English using a large text - War and Peace.

Credits:
This exercise has been designed by Dr Maneesh Sahani as part of the Approximate Inference and Learning in Probabilistic Models module taught at UCL.
