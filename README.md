# judge_float
python_


print 'welcome to the receipt program!'
total = 0
while 1:
    pri = raw_input('Enter the value for the seat [\'q\' to quit]: ')
    if pri == "q":
        break
    try:
        pri = float(pri)
        total = total + pri
    except ValueError:
        print 'I\'m sorry, but {} isn\'t valid. Please try again.'.format(pri) 
print '*' * 5
print 'Total: ${}'.format(total)
