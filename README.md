When a field is declared as volatile, then, the Java Memory Model ensures that all threads will “see” the same consistent value.

In Java, a global ordering is imposed on the read and write operations concerning a volatile variable. A thread that access a volatile field, will first read its current value from the main memory, instead of using a potential cached value. A write operation to a volatile variable establishes a happens-before relationship with all subsequent reads of that volatile variable. Therefore, any change to a volatile variable is always visible to other threads.
