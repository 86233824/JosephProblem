#  Python3基础算法：Joseph Problem
约瑟夫环（约瑟夫问题）是一个数学的应用问题：已知n个人（以编号1，2，3...n分别表示）围坐在一张圆桌周围。从编号为k的人开始报数，数到m的那个人出列；他的下一个人又从1开始报数，数到m的那个人又出列；依此规律重复下去，直到圆桌周围的人全部出列。



    # -*- coding = utf-8 -*-
    a = [x + 1 for x in range(10)]  # 人数为10人，编号1~10
    index, step = 0, 3    # 数到3的人出列
    while len(a) > 1:
        index = (index + s - 1) % len(a)  
        print('kill No.', a[index])
        del a[index]
    print('\nWinner is', a[0])
  
