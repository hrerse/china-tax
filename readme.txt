��ȡ�ļ�ʹ��python���÷���open()���ļ���ʹ��.read()��ȡȫ�����ݣ�ʾ�����£�

path = "c:\doc\py.txt"
fi = open(path, "r")
print(fi.read())
fi.close()
with�﷨

with��python2.5������Զ��ͷ���Դ���﷨ģʽ��ȷ��ʹ�ù����в����Ƿ������쳣�������ͷ���Դ. ʹ��with��ȡ�ļ����ǲ���Ҫ�Լ��ֶ�close�ģ�ʾ�����£�

with open(path) as fi:
    print(fi.read())
���ж�ȡ�ļ� .read()�Ƕ�ȡ�ļ���ȫ�����ݣ�ʹ��.readlines()��ʾ�����£�

with open(path, "r") as fi:
    lines = fi.readlines()
print(len(lines))
open������ģʽ

�����ʾ�����Կ�������open(Ŀ¼,����ģʽ)��ʱ�����ָ������ģʽ��open�Ĳ���ģʽ��

��ȡģʽ��'r'(Ĭ��ģʽ) | д��ģʽ��'w' | ����ģʽ��'a'.

pythonģʽ�Ƕ�ȡ������"r"����ʡ�ԣ�ʾ�����£�

path = "c:\py.txt"
fi = open(path)
print(fi.read())
fi.close()