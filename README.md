# A file-based key-value data store that supports the basic CRD

## Walkthrough
import code as x  <br>
x.create("amrita",25) <br>
x.create("src",70,3600) <br>
x.read("amrita") <br>
x.read("src") <br>
x.create("amrita",50) <br>
x.modify("amrita",55) <br>
x.delete("amrita") <br>
t1=Thread(target=(create or read or delete),args=(key_name,value,timeout)) #as per the operation <br>
t1.start() <br>
t1.sleep() <br>
t2=Thread(target=(create or read or delete),args=(key_name,value,timeout)) #as per the operation <br>
t2.start() <br>
t2.sleep() <br>
