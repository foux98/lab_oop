**Kata**:

https://www.codewars.com/kata/51e0007c1f9378fa810002a9/train/python

Remove All The Marked Elements of a List

    def remove_(self, integer_list, values_list):
            return [x for x in integer_list if x not in values_list]


```python
https://www.codewars.com/kata/56311e4fdd811616810000ce/train/python
```

#Method For Counting Total Occurence Of Specific Digits

class List:
    def count_spec_digits(self, integers_list, digits_list):
       
        digit_freq = {digit: 0 for digit in digits_list}

       
        for num in integers_list:
          
            num_str = str(abs(num))
           
            for digit in digits_list:
                digit_freq[digit] += num_str.count(str(digit))

        
        result = [(digit, digit_freq[digit]) for digit in digits_list]

        return result

#Ordered Count of Characters

https://www.codewars.com/kata/ordered-count-of-characters

def ordered_count(inp):
   
    char_count = {}
    
   
    for char in inp:
       
        char_count[char] = char_count.get(char, 0) + 1
    
    
    result = [(char, count) for char, count in char_count.items()]
    
    return result
