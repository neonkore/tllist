# tllist

**tllist** is a **T**yped **L**inked **L**ist C header file only
library implemented using pre-processor macros.


## Usage

### Declaring a variable, or defining a type:

1. Declare a variable

   ```c
   tll(int) an_integer_list;
   ```


2. Typedef

   ```c
   typedef tll(int) an_integer_list_t;
   an_integer_list_t an_integer_list;
   ```

3. Named struct

   ```c
   tll(int, an_integer_list);
   struct an_integer_list an_integer_list;
   ```
