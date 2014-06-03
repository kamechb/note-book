# mysql 

## 读写控制

mysql 在读的时候会创建共享锁(读锁)，在写的时候会创建排他锁(写锁)

## mysql 并发控制

### mysql 分4个隔离级
* read uncommited
* read commited
* repeatable read(默认)
* searializable

在repeatable read level 也会产生phatom read(幻读), 它是通过mvcc机制防止了幻读

详情见高性能mysql第一章

注：mysql在repeatable read level 结合mvcc机制防止了幻读，
但是仍不能防止多进程（线程）并发的读写数据，导致数据的覆盖问题，
该问题可以通过乐观锁解决, 同时rails提供了乐观锁的支持。
