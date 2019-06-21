# inverse-generator

输入包含规律的数值串,解析如果成功返回对应生成器，失败则返回false

----
输入要求：数值串的每两个前后数值间，存在任意的加减规律。
例：[1,3,5,7,9] ->数字规律+2
例：[-1,2,-3,4] ->数字规律+1，正负规律-,+,-,+,-...
算法：用两个维度（数值在数轴上变化的方向、距离）概括规律数值串的一切变化,由此反向生成该数值串的生成器。

用法：
输入：包含规律的数值串
返回：对应的生成器
例如：输入[1,3,6,10]，返回生成器，用于生成[1,3,6,10,15,21...以及其后所有数值]

其它相关：
暂时不支持乘法规律解析，输入[1,2,4,8]将返回false
暂时不支持视觉规律解析，输入[1,22,333,4444]将返回false
