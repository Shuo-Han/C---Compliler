# Conventions

- Stack pointer always points to the next available slot. i.e. `$sp+4` is the top element.
- Func call:

      ...
      func_param_2
      func_param_1
      $ra            <- $fp
      $old_fp
      local_var_1
      local_var_2
      ...
      local_var_n
      unused         <- $sp

# Implemented Functions:
- [x] `main` function check done in `nameAnalysis`
- [x] local/formal offset relative to `$fp`
- [x] global var label name allocation done in `nameAnalysis`
- [x] all variables are assumed to be 4 bytes since we only have int and bool
