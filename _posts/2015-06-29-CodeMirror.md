
---
layout: post
title: CodeMirror-SQLHintʹ��
---

��������ʹ�ó�����Ӧ����Ҫ�ṩһ���򵥵�SQL��ѯ���ڣ��ܹ�������ʾSQL�﷨���ɡ�
##### 1. ��ȡ������������
   ��codemirror��������������һ�״��룬��lib�µ�```codemirror.js��codemirror.css```�ļ���mode/sql�ļ����µ�```sql.js```�ļ����뵽ҳ���С�lib��codemirror��lib��mode�ǵ�ǰʹ�õ�����ģʽ����SQL���ԡ�
##### 2. ���ʹ��
   ����Ĵ���չʾ����γ�ʼ��һ��codemirror���Լ���Ĳ����������塣
 ```
<!-- Create a simple CodeMirror instance -->
<link rel="stylesheet" href="lib/codemirror.css">
<script src="lib/codemirror.js"></script>
<script src="mode/sql/sql.js"></script>
<script>
  var editor = CodeMirror.fromTextArea(myTextarea, {
    lineNumbers: true,//�����к� boolean
    value: 'SELECT * FROM table',//�༭���ʼֵ string    
    mode: 'text/x-mysql',//��ǰcodeģʽ ģʽ��ѡ�������CodeMirror.modes�в鿴

  });
</script>
```