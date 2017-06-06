
#import
import rbt as rb
import numpy as np
rbt = rb.REDBLACKTREE()
results = []
not_found = []


with open('input.txt') as inputfile:
    for line in inputfile:
        x = int(line)
        if x > 0:
            rbt.rb_inserting(rb.Nd(x))
        elif x < 0:
            min = rbt.b_search(rbt.root, np.absolute(x))
            if min == -1:
                not_found.append(x)
            else:
                rbt.rb_delete(min)
        else:
            rbt.count_nd()
            rbt.inorder_iterary(rbt.root)
            print(" ")
            break

inputfile.close()
