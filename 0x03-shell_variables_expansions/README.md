0-alias
#!/bin/bash
alias ls="rm *"
1-hello_you
#!/bin/bash
echo "hello $USER"
2-path
#!/bin/bash
export PATH=$PATH:/action
3-paths
#!/bin/bash
echo $((`echo $PATH | grep -o ":/" | wc -l`+ 1))
4-global_variables
#!/bin/bash
printenv
5-local_variables
#!/bin/bash
set
6-create_local_variable
#!/bin/bash
BEST="School"
7-create_global_variable
#!/bin/bash
export BEST=School
8-true_knowledge
#!/bin/bash
echo $(($TRUEKNOWLEDGE + 128))
9-divide_and_rule
#!/bin/bash
echo $(($POWER / $DIVIDE))
10-love_exponent_breath
#!/bin/bash
echo $((BREATH**$LOVE))
11-binary_to_decimal
#!/bin/bash
echo "$((2#$BINARY))"
12-combinations
#!/bin/bash
echo {a..z}{a..z} | tr " " "\n" | grep -v "oo"
13-print_float
#!/bin/bash
printf "%.2f" $NUM | sort
100-decimal_to_hexadecimal
#!/bin/bash
printf '%x\n' $DECIMAL
101-rot13
#!/bin/bash
tr 'A-Za-z' 'N-ZA-Mn-za-m'
102-odd
#!/bin/bash
perl -lne 'print if $. % 2 ==1'
103-water_and_stir
#!/bin/bash
echo $(printf %o $(($((5#$(echo $WATER | tr 'water' '01234'))) + $((5#$(echo $STIR | tr 'stir.' '01234'))))) | tr '01234567' 'bestchol')
