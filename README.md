# Test Driven Ranges

This exercise extends the [Battery Monitoring] use-case.

The charging current varies during the process of charging.
We need to capture the range of current measurements -
what range of currents are most often encountered while charging.

> **DO NOT** jump into implementation! Read the example and the starting task below.

## Example

### Input

Consider a set of periodic current samples from a charging session to be:
`3, 3, 5, 4, 10, 11, 12`

### Functionality

The continuous ranges in there are: `3,4,5` and `10,11,12`.

The task is to detect the ranges and
output the number of readings in each range.

In this example,

- the `3-5` range has `4` readings
- the `10-12` range has `3` readings.

### Output

The expected output would be:

```
Range, Readings
3-5, 4
10-12, 3
```

## Tasks

Start test-driven development:

1. Establish quality parameters for your project: What is the maximum complexity you would allow? How much duplication would you consider unacceptable? What is the coverage you'll aim for?
Adapt/adopt/extend the `yml` files from one of your workflow folders.

1. Write the smallest possible failing test.
   
   #include <vector>
  
   <vector> int reading;
   <vector> int minimum; 
   <vector> int maximum;
   <vector> int count;
      
   Test(RangeTrends, BasicTest)
   {
   FindRangeTrends(reading,minimum,maximum,count);
   };

1. Write the minimum amount of code that'll make it pass.

    #include <vector>
    
    void FindRangeTrends(<vector> &f_count, <vector> &f_minimum, <vector> &f_maximum, <vector> &f_reading)
    {
    }

1. Write the next failing test.

Implement one failing test and at least one passing test:


