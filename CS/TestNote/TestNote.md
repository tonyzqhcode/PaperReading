
# A Test Is Successful if the Program Fails

If a set of tests does not produce any failure, we are either in the extremely unlikely case of a correct program, or in the very likely situation of a bad set of tests that are not
able to reveal failures of the program.

# Failure, Fault, and Error
![TestGoal](TestType.png)


# Testing Methods:Black-box Testing And White-box Testing

![Black_white](black_white.png)

**Black-box Testing
- Based on a description of the specification/business need
- Cover as much specified behavior as possible
- Do not start with implementation details

**White-box Testing
- Based on the code
- Cover as much as coded behavior as possible

Quiz:
	If you created a table,which method will you use to check quality?
	If a data enginner build a table for you to enable a critical analysis,which method will you use to check quality?


# White-box Testing: Is 100% Code/Statment Coverage Enough to Reveal All Faults?

Coverage measure = number of executed statments /total number of statements 

Note:"Typical coverage" target is 80-90%.

```java

    public static int weakMethod2(int a) { 

        int b=0;

        if (a>0) {
            b = 1;
        }

    return a/b;
    
    }

```

Will test case `a=1` achieves 100% statement coverage? Can this case reveal error?

# Testing Granularity Levels
![TestGranularity](TestGranularity.png)