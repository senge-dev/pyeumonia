# Pyeumonia

�¹ڷ�������API�����Դ�[����԰����](https://ncov.dxy.cn/ncovh5/view/pneumonia)��ȡ�������ݡ�

## ��װpypi

��װpypi��:

```bash
pip install pyeumonia
```

## �Զ�����

������Ѿ���װ��pyeumonia���������İ汾��`0.1.0a0`�£������Զ������£���Ҳ���԰������²������ò�����ʵ���Զ����¡�

```python
from pyeumonia.pyeumonia import Covid
covid = Covid(check_upgradable=True, auto_update=True)
```

����㲻���Զ������£�������������:

```python
from pyeumonia.pyeumonia import Covid
covid = Covid(check_upgradable=False)
```

��������ֶ�������������ʹ��`pip install --upgrade pyeumonia`��

## ���ʹ��

### ��ȫ������������

```python
from pyeumonia.pyeumonia import Covid
covid = Covid(language='zh_CN')
data = covid.world_covid_data()
```

### ��ȡĳ�����ҵ�������Ϣ��

```python
from pyeumonia.pyeumonia import Covid
covid = Covid(language='zh_CN')
# ��ȡ�ձ���30���������Ϣ
data = covid.country_covid_data(country_name='Japan', show_timeline=30)
```

### ��ȡ���ڵ�������Ϣ

```python
from pyeumonia.pyeumonia import Covid
covid = Covid(language='zh_CN')
# ��ȡ���ڵ�������Ϣ
data = covid.cn_covid_data()
```

### ��ȡ����ĳ��ʡ/������/ֱϽ��/�ر���������������Ϣ

```python
from pyeumonia.pyeumonia import Covid
covid = Covid(language='zh_CN')
# ��ȡ�㽭ʡ��30���������Ϣ������ȡ��ǰ�������е�������Ϣ
data = covid.province_covid_data(province_name='�㽭', show_timeline=30, include_cities=True)
```

### ��ȡ���ڵ��и߷��յ���

```python
from pyeumonia.pyeumonia import Covid
covid = Covid(language='zh_CN')
# ��ȡ���ڵ��и߷��յ���(����ʾ���ڵķ��յ�������)
data = covid.danger_areas_data(include_cities=False, include_counts=False, include_danger_areas=True)
```

## ����Դ�������

������ʹ��[GNU GPL v3](https://jxself.org/translations/gpl-3.zh.shtml)��Դ���������������

- �������Ѹ��Լ���python����ʹ�ñ������Դ���롣
- ����ԶԱ���������޸ĺͷַ��������뱣�����������˵����ԭ������Ϣ
- ���۳����κ�Ŀ�ģ��������ֹ������ҵ��;����������������ҵ��վ����ҵӦ�á���ҵ�ƹ�ȡ�
