# tllist

**tllist** is a **T**yped **L**inked **L**ist C header file only
library implemented using pre-processor macros.


## Usage

### Declaring a variable, or defining a type:

1. **Declare a variable**

   ```c
   /* Declare a variable using an anonymous type */
   tll(int) an_integer_list;
   ```


2. **Typedef**

   ```c
   /* First typedef the list type */
   typedef tll(int) an_integer_list_t;

   /* Then declare a variable using that typedef */
   an_integer_list_t an_integer_list;
   ```

3. **Named struct**

   ```c
   /* First declare named struct */
   tll(int, an_integer_list);

   /* Then declare a variable using that named struct */
   struct an_integer_list an_integer_list;
   ```
