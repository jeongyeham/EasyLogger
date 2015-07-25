# stm32f10x RT-Thread Demo

---

## 1�����

ͨ�� `app\src\app_task.c` �� `test_elog()` ������������־��������û����Խ����ն���������־�����������������á�

### 1.1��ʹ�÷���

�򿪵��Ե��ն���Demo�Ĵ���1�������ӣ��������� 115200 8 1 N����ʱ���ն��оͿ������� "2.6 Demo" Gif�������ᵽ�ĳ���������£�

- 1��elog��ʹ����ʧ�������־��elog on��ʹ�ܣ�elog off��ʧ��
- 2��elog_lvl�����ù��˼���(0-5)��
- 3��elog_tag�����ù��˱�ǩ�����ú���ֻ�е���־�ı�ǩ�������˱�ǩʱ���Żᱻ����������κβ�������չ��˱�ǩ��
- 4��elog_kw�����ù��˹ؼ��ʣ����ú���ֻ�е���־�� **��������** �������˹ؼ���ʱ���Żᱻ����������κβ�������չ��˹ؼ��ʡ�

## 2���ļ����У�˵��

`components\easylogger\port\elog_port.c` ��ֲ�ο��ļ�

`RVMDK` ��ΪKeil�����ļ�

`EWARM` ��ΪIAR�����ļ�

## 3����������

- 1������ RTT���Լ�Ӳ���쳣�Ĺ��ӷ�����ʹ��ϵͳ�ڳ����쳣ʱ��������־��Ȼ���Ա�����򱣴档�ο� `app\src\app_task.c` �е� `rtt_user_assert_hook` �� `exception_hook` ������
- 2������ EasyLogger���ԵĹ��ӷ�����ʹ��ϵͳ�ڳ����쳣ʱ��������־��Ȼ���Ա�����򱣴档�ο� `app\src\app_task.c` �е� `elog_user_assert_hook` ������