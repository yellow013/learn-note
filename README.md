Share0 —— Cassandra database & Time series data
-
0.NoSQL数据库概述
- RDB的局限性
	- ACID事务
		- 原子性(**A**tomicity)
		- 一致性(**C**onsistency)
		- 隔离性(**I**solation)
		- 持久性(**D**urability)
	- RDB存储方式
	
- CAP定理
	 - 一致性(**C**onsistence) (等同于所有节点访问同一份最新的数据副本)
	- 可用性(**A**vailability) (每次请求都能获取到非错的响应——但是不保证获取的数据为最新数据)
	- 分区容错性(**P**artition tolerance) (以实际效果而言，分区相当于对通信的时限要求。系统如果不能在时限内达成数据一致性，就意味着发生了分区的情况，必须就当前操作在C和A之间做出选择)
	
- **N**ot **O**nly **S**QL

- NoSQL数据库类型以及特性
	- 文档型数据库(Document) (MongoDB, CouchDB)
	- 键值型数据库(Key-Value) (Redis)
	- 列式数据库(Column) (Cassandra, HBase)
	- 图数据库(Graph) (Neo4j)

1.Cassandra介绍
- 来历
	- Facebook开源
	- 集合Google BigTable的数据模型与Amazon Dynamo的P2P结构
- 数据模型
	- Column (name<byte[]>, value<byte[]>, timestamp<?>)
	- Super Column (name<byte[]>, value<Column<?>>)
	- Column Familes(Column[?])
	- Row (Column)
	- Keyspace
	- Sorted
- 特性
	- 高性能写入
	- 顺序索引查询 
	- CQL查询语句
	- CAP属性可调

2.时序数据
- 数据结构特性
- 存储特性

3.基于Cassandra的时序数据库
- 自建存储模型与索引
- 使用KairosDB


Share1——Concurrent programming & Thread safety
-
0.并发编程模型
- 线程与锁
- Actor模型
- SCP模型
- STM模型

1.常用技术
- Lock
- CAS
- Queue
- ThreadLocal
- ……
