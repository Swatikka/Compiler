ConstantPropagation

  For the given block of statements, three address statement,basic block and DAG are generated. Constant folding occurs and the new three address statement is generated.
  
ControlFlowGraph

  For the given block of statements, three address statement, basic block and control flow graph are generated.
  
Syntax tree
  
  For the given arithmetic expression, syntax tree is created.
  
boolean backpatching
  
  For the given boolean expression, truelist,falselist are generated.
  
forwhile
  
  "while" statement is generated for the given "for" statement.
  
ifelse
  
  For a given "if" statement, corresponding "else" statement is added if not present.
  
labelledtree
  
  For the given arithmetic expression, labelled tree is generated.
  
symboltable
  
  For the given declaration statements, symbol table is generated.
  
      
      
How to compile
      open the terminal
      
      lex filename.l
      
      yacc -d filename.y
      
      gcc lex.yy.c y.tab.c -ll (for the folders Syntax tree, forwhile, ifelse, symboltable)
      
      ./a.out
      
      g++ lex.yy.c y.tab.c -lfl (for the folders ConstantPropagation,ControlFlowGraph,boolean backpatching, labelled tree)
      
      ./a.out<input text file
