r3c����redis�ٷ���c��hiredisʵ�֣�ȫ����redis cluster C++ client��֧��redis cluster��

��������r3cʱ��Ĭ����Ϊhiredis�İ�װĿ¼Ϊ/usr/local/hiredis��
��������ִ��makeʱָ��hiredis��װĿ¼�������hiredis��װĿ¼Ϊ/tmp/hiredis��make HIREDIS=/tmp/hiredis��
���޸�Makefile�б���HIREDIS��ֵ��ָ��hiredisʵ�ֵİ�װĿ¼��

����r3c�ɹ��󣬽�����libr3c.a��̬�⣬û�й���ⱻ���ɡ�
Ҳ����ֱ�ӽ�r3c.h��r3c.cpp�����ļ����뵽�Լ���Ŀ������һ����룬������������r3c��

r3c_cmd.cpp��r3c�ķǽ���ʽ�����й��ߣ��߱�redis-cli��һЩ���ܣ����÷�������ͬ�����𲽽�����redis-cli�����й��ܡ�
r3c_test.cpp��r3c�ĵ�Ԫ���Գ�������make test���ɡ�

����r3c��
make

��װ��PREFIXָ����װĿ¼�������ָ����Ϊ/usr/local����
make install PREFIX=/usr/local/r3c

ִ�е�Ԫ���ԣ�
make test

����Դ������������
make dep
