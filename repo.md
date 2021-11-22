# homework repo
## Answer 1
$ md5sum test.txt|cut -d ' ' -f1
'''test.txt is a created text file'''

## Answer 2
$ diff test.txt test2.txt
'''test.txt is from answer 1, test2.txt is from answer 2'''

## Answer 3
function odd-or-even(){
reg_int='^[1-9][0-9]*$|^[-][1-9][0-9]*$|^0$'
if [[ "$1" =~ $reg_int ]] ; then
	    if [ $(($1 % 2)) == 0 ] ; then
		         echo "even"
			     else
				          echo "odd"
					      fi
				      else
					          echo "Not a Number"
fi
}
