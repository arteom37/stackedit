$f(x, y) = \frac{1}{x} + \frac{1}{y}$
$F(x, y) = x + y - 1 = 0$
Подставляем $y = 1 - x$ в $f$

${f(x, y = 1 - x)} = \frac{1}{x} + \frac{1}{1-x}$
$f'(x) = -\frac{1}{x^{2}}+ \frac{1}{(1-x)^{2}}$
Нуль в $x = \frac{1}{2}$, несложно убедиться, что это локальный минимум.
В $x = 0$ и $x = 1$ нуль кратности два и экстремума там нет.
Т.е. $x_{0} = \frac{1}{2}$, а $y_{0} = \frac{1}{2}$, а локальный минимум в $f(x_{0}, y_{0}) = 4$.

Если $x < 0$ или $ x >1$, то видно, что $f(x) < 0$.

Можно и так:
Лагранжиан
$L(x, y, \lambda) = \frac{1}{x} + \frac{1}{y} + \lambda(x+y-1)$.
$\frac{\partial L}{\partial x} = -\frac{1}{x^{2}} + \lambda$
$\frac{\partial L}{\partial y} = -\frac{1}{y^{2}} + \lambda$
$x+y - 1 = 0$

Тогда из первых двух уравнений $x^{2} = y^{2}$, т.е. $x = \pm y$.
Подставляем в третье:
$x = y => y = x = \frac{1}{2}$
$x = - y$ -- так не бывает.
Значит подозрительная точка $(x, y) = \frac{1}{2}$.

Достаточное условие: 
$d^{2}L = L_{xx}(dx)^{2}+ 2L_{xy} (dxdy)+ L_{yy}(dy)^{2}$
Пусть$$ S = \{ (x, y) | x + y - 1 = 0 \}$$
Тогда $T_{p}S \subset T_{p}{\mathbb{R}^{2}}$
Посмотрим на ограничение $d^{2}{L}$ на $T_{p}(S)$.
Т.к. $x + y - 1 = 0$, то $dx + dy = 0$, т.е. $dy = -dx$.
Подставляем в второй дифференциал.
$$d^{2}{L}|_{S} = L_{xx}(dx)^{2} - 2L_{xy}(dx)^{2} + L_{yy} (dx)^{2} = (L_{xx} - 2L_{xy}+L_{yy})(dx)^{2}$$

Знакоопределенность этой формы и даст достаточное условие экстремума.
ОК, тогда $L_{xx} = \frac{2}{x^{3}}$, $L_{xy} = 0$, $L_{yy} = \frac{2}{y^{3}}$
Тогда 
$$d^{2}{L}|_{S}(\frac{1}{2}, \frac{1}{2}) = (16+16)(dx)^{2} = 32(dx)^{2} > 0$$ значит, тут локальный минимум.
Раз множителей Лагранжа больше нет, то и локальных минимумов/максимумов тоже больше нет.

