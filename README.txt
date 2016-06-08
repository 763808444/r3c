Redis Cluster C++ Client, based on hiredis and support standalone, it's easy to make and use, not depends on C++11 or later.

r3c����redis�ٷ���c��hiredisʵ�֣�ȫ����redis cluster C++ client��֧��redis cluster��

��������r3cʱ��Ĭ����Ϊhiredis�İ�װĿ¼Ϊ/usr/local/hiredis��
��������ִ��makeʱָ��hiredis��װĿ¼�������hiredis��װĿ¼Ϊ/tmp/hiredis��make HIREDIS=/tmp/hiredis��
���޸�Makefile�б���HIREDIS��ֵ��ָ��hiredisʵ�ֵİ�װĿ¼��

����r3c�ɹ��󣬽�����libr3c.a��̬�⣬û�й���ⱻ���ɡ�
Ҳ����ֱ�ӽ�r3c.h��r3c.cpp�����ļ����뵽�Լ���Ŀ������һ����룬������������r3c��

r3c_cmd.cpp��r3c�ķǽ���ʽ�����й��ߣ�command line tool�����߱�redis-cli��һЩ���ܣ����÷�������ͬ�����𲽽�����redis-cli�����й��ܡ�
r3c_test.cpp��r3c�ĵ�Ԫ���Գ���unit test����ִ��make test���ɡ�

����r3c��Compile r3c����
make
��or��
make HIREDIS=/tmp/hiredis

��װ��PREFIXָ����װĿ¼�������ָ����Ϊ/usr/local����
make install
��or��
make install PREFIX=/usr/local/r3c

ִ�е�Ԫ���ԣ�
make test
��or��
make test REDIS_CLUSTER_NODES=192.168.31.11:6379,192.168.31.11:6380

����Դ������������
make dep

���ڽӿڣ�
�������CRedisClient��nodes����Ϊ�����ڵ��ַ�������192.168.0.1:6379��Ϊ����ģʽ��Ϊ��ڵ��ַ���ʱ��ΪRedis Clusterģʽ��
