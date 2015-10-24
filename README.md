# ����� ������������� HeadHunter. �������� ������� 2015. ������ ���

����� �������: �������� ���������
<mailto:iskuskov@gmail.com>

����������� **Python 2.7**

--------

## ������ � 1. ����������� ����������

### �������
��� ����� �� N ����� �� ��������� (��� �������� ����� �������, ��� � ���� ����� ������������� ����������). ������� ����������� ���������� ����� ����� ������� �� ����� ������.

������ ������� ������:<br>
10 10<br>
20 10<br>
20 15<br>

������ �������� ������:<br>
5

### �������� �������

�������������� ���������� �� ��������� ��� ��������������� ������� �� ���������� $x$ � $y$ (����� ������ � $O(n\log n)$), ����� ���� �������� ����������� �������, ������������ ����������� ���������� ����� �������.

� ����������� ������� �������� ������ ����� �� ��� ����� ������������ ������������ ������� (�� $O(n)$) � ���������� ������ � ������ �� ������ ����������� ����������. ������� ���������� ����������, ��������� �� ������ ������, $?$.

�������� ���������, ��� �� �����, ������� � ������ ��������� ������� ���������� ������, ��� $?$. ��� ����� ���������� ����� ����� � �������, ��� ���� ���� �����, ���������� �� ������� ������, ��� $?$, ��� ���������� ������ ������ � �������������� �� ��������� $?$ �� $2?$, ����� �������� �������� ����� ��������� ������������ ����� ������������ ������.

��� ��� � ����� �������������� ����� ���������� �� ����� ������ ����� (����� ���������� ����� ���� ������ ������ $?$ � ��������� ������������), �� ��� ������ ����� ����������� ���� 7 �����, ������������� ����� ������� � ��������������� �� y ������� �����, ������� � ������ $�?$ ������������ ������������ ������.

����� ����� ������ ���������: $T_{rec}[n]=2T_{rec}[n/2]+O(n)=O(n\log n), T[n]=O(nlogn)+T_{rec}[n]=O(n\log n)$

### ������ ������� ������

������������ � �������������� �������� ��������� - ���� � �����, � ������� ���������� ������ �����. � ������ ���������� ������� ���������, ���� �������������� � ���������� �� ��������� ������ ������ ������.

���������� ����� ������ ���� ������� ����� ������, ������ ����� �� ��������� ������ (��� � �����, ��� � ��� ����� � ����������). 
��� ������� ��. "points.txt". ������ ���� ������� ��� ������� 2 �����, � ��������� ������ ������� ������ �� ����� ������ (����� ���������� ����������� ��������).

������ ������������� ���������:
`python minimal_distance.py points.txt`

### ������ �������� ������

� ����������� ����� ���������� �����, ���������� ����������� ����������� ����� ����� ������� �� ������. ���� ����� ������� �����, ��� �� ���� �����, ����� ���������� ����������� ��������


--------

## ������ � 2. ���������� ��������� �� k ���������

### �������

��� ������ ����������� ����� n � k ���������� ���������� �������� ����������� ����� n � ���� ����� k ����������� ���������, ���� �������, ������������ ������ �������� ��������� ������� �����������.
��������� �������� �� ���� ��� ����������� ����� n � k, �� ������������� 150.

������ ������� ������:<br>
6 3

������ �������� ������:<br>
3


### �������� �������

��� ������� ������ ���� ������������ ��������� *������������ �������*:

$p(n,k) = p(n-1, k-1) + p(n-k, k)$, ���

$p(n-1, k-1)$ - ���������� ���������, ���������� ����� ������� ����� 1, 

$p(n-k, k)$ - ���������� ������ ��������� (���� ���������� ����� �� ������ 2, ����� ������� �� ������ ����� �� 1 �, ����� �������, �������� ��������� $n-k$ �� $k$ ������)


*���� ��������*:

$p(i,i) = 1$

$p(n,1) = 1$

$p(n,k) = 0$ ��� $k > n$

��� �������������� ��������� ���������� ������������ ����������.


### ������ ������� ������

��������� �������� �� ���� ��� ������������� ��������� - ����� n � k. � ������ ���������� ������ ����������, ���� n � k �������������� � ���������� ����� ������.

������ �������������: `python partition_count.py 6 3`


### ������ �������� ������

� ����������� ����� ���������� ����� �����, ���������� �������.

-------