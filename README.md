# Python-Code-Building-New-Array-from-Unique-Elements-in-Two-Arrays

  - The `build_new_array` function is defined to take two arrays (`array1` and `array2`) as input parameters.

   - Inside the function, the input arrays `array1` and `array2` are converted into sets (`set1` and `set2`, respectively). This conversion is done to facilitate efficient membership testing, as sets offer constant-time average complexity for checking membership.

   - The function then uses list comprehension to build a new array (`new_array`) containing elements that are only present in one of the input arrays. This is achieved using the following steps:
     - For each element `x` in `array1`, it checks whether `x` is not present in `set2`. If `x` is not in `set2`, it means `x` is unique to `array1`, so it is added to `new_array`.
     - Similarly, for each element `x` in `array2`, it checks whether `x` is not present in `set1`. If `x` is not in `set1`, it means `x` is unique to `array2`, so it is also added to `new_array`.
     - By doing this, `new_array` contains elements that are unique to either `array1` or `array2`, but not both.

   - Finally, the function returns the `new_array`, which contains the desired result.

   - An example usage of the function is provided, where it is called with two sample arrays (`array1` and `array2`). The result array (`result_array`) is printed to demonstrate the unique elements present in either of the input arrays.
