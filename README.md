# A file-based key-value data store that supports the basic CRD

## Walkthrough
import code as x 
x.create("amrita",25)
x.create("src",70,3600) 
x.read("amrita")
x.read("src")
x.create("amrita",50)
x.modify("amrita",55)
x.delete("amrita")
t1=Thread(target=(create or read or delete),args=(key_name,value,timeout)) #as per the operation
t1.start()
t1.sleep()
t2=Thread(target=(create or read or delete),args=(key_name,value,timeout)) #as per the operation
t2.start()
t2.sleep()