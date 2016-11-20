(a)
~~~
s2 = 0
s3 = s0

while s3 != 0:
  s2 += s1
  s3 -= 1
~~~

(b) s3 equals s0 so the loop will play s0 number of times and within the loop s1 is being added into s2 therefore s1 is being multiplied
s0 number of times, storing the result in s2.

(c)
~~~
s0 = 10
s1 = 1

while s0 != 0:
  s2 = 0
  s3 = s0
  while s3 != 0: 
    s2 += s1
    s3 -= 1
  s1 = s2
  s0 -= 1
~~~

(d) s3 is equal to s0 therefore the inner and outer loop all depend on what the value of s0 is, storing the factorial value in s2 first
then transfering it into s1, subtracting 1 from s0 before the start of the next loop. For example in the first loop s1 = 1 and if s0 = 10,
s3 will be the same value as s0 which is 10 then add 1 from s1 10 times into s2, storing the value 10 from s2 to s1, subtract one from s0
and starting the loop again, reseting s2 to 0, s0 = 9, s3 = s0 but keeping the new value of s1, adding s1 to s2 nine times, storing the
value of s2 to s1, subtract 1 from s0, reset s2 to 0, s0 = 8, s3 = s0 add s1 (90) to s2 eight times and so on until s0 = 0.
So the equation would look like 10 * 9 * 8 * 7 * 6 etc and s1 will equal 3628800.

(e)
~~~
        addi $s0, $szero, 10
        addi $s1, $szero, 1
inner:  mult $s1, $s0
        mflo $s1
        addi $s0, $s0, -1
        bne $s0, $szero, inner
~~~
