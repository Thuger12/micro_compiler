# Compiler for C
Start exciting journey. Use Haskell for that(pattern matching, functional language...).
Start from basic model of compiler and write module after module.

Basic structure is:
  - Lexical analyzer(simple tokens analyz)
    * Regular expression and FSM
    * Think about DFA vs NFA
    * REGex into DFA
    * NFA into DFA
    * Backtracking
    * Plan:
        - Tokenizer by DFA(scan main keywords, signs, data types and id's)
  - Parser(output is parse tree)
    * Context free grammar, Parser types(TD, BU), types of grammar itself.
    * TopDown vs BottomUp 
    * LL vs LR
    * LL is easy to write, but harder to build(left recursion and prefixes)
    * Build SLR parser:
        - Create LR(0) automaton
        - Find follow and first
        - Create Parse Table from this
        - Write parser(stack, parse table, parser itself)
  - Semantic analyzer(It's all about semantic correctness)
  - Intermediate code representation
  - Code optimizer
  - Assembly output
