(1) По определению
$R(X, Y)Z = \nabla_{X} \nabla_{Y}Z - \nabla_{Y} \nabla_{X}Z - \nabla_{[X, Y]}{Z}$, где $X, Y \in S(TM, M)$ -- гладкие сечения касательного расслоения (векторные поля).

Надо доказать, что 
$R(X, Y)Z+R(X, Z)Y+R(Y, Z)X=0$
Заметим, что достаточно доказать в голономном базисе $\{\frac{\partial}{\partial x_{i}}\}$ (в таком случае все скобки $[\frac{\partial}{\partial x_{i}}, \frac{\partial}{\partial x_{j}}] = \delta_{ij}$

Пусть $X, Y$ -- базисные вектора, тогда $R(X, Y)Z+R(X, Z)Y+R(Y, Z)X = \nabla_{X} \nabla_{Y}Z - 
\nabla_{Y} \nabla_{X}Z + \nabla_{X} \nabla_{Z} Y - \nabla_{X} \nabla_{Z} Y + \nabla_{Y} \nabla_{Z} X - \nabla_{Z} \nabla_{Y} X = 0$, т.к. связность Леви-Чивита без кручения, т.е. $\nabla_{X}{Y} = \nabla_{Y}{X}$

(2) Задача -- доказательство в одну сторону основной теоремы римановой геометрии.

*Утверждение* 
Пусть $\nabla_{X}{Y}$ -- связность Леви-Чивиты в касательном расслоении $TM$, где $X, Y \in S(TM, M)$ -- гладкие сечения.
Тогда выполнено соотношение из задачи.

*Доказательство*
Достаточно доказать, что для всякой римановой метрики $g \in S^{2}(T^{*}M \otimes T^{*}M)$ и связности Леви-Чивита (т.е. связности без кручения, которая согласована с метрикой), выполнено равенство.

Из условий согласованности следует:

$X \langle Y, Z \rangle = \langle \nabla_{X}{Y},  Z\rangle + \langle Y, \nabla_{X}{Z} \rangle$
$Y \langle Z, X \rangle = \langle \nabla_{Y}{Z}, X \rangle + \langle Z, \nabla_{Y}{X} \rangle$
$Z \langle X, Y \rangle  = \langle \nabla_{Z}{X}, Y \rangle + \langle X, \nabla_{Z}{Y} \rangle$

Т.е. $\nabla$ без кручения, то и 
$$X \langle Y, Z \rangle - Z \langle X, Y \rangle + Y \langle Z, X \rangle = 2 \langle \nabla_{X}{Y}, Z \rangle - \langle [X, Y], Z \rangle + \langle Y, [X, Z] \rangle + \langle X, [Y, Z] \rangle$$, что и доказывает утверждение.

(связность Леви-Чивиты -- это такая связность, что (1) \nabla G = 0 (согласованность с метрикой) (2) Torsion-free condition, т.е. \nabla_{X}{Y} - \nabla_{Y}{X} = [X, Y] (последнее свойство также назявается симметрической связностью, т.к. если $\{ \frac{\partial}{\partial x_{i}}\}$ -- голономный базис, то $[\frac{\partial}{\partial x_{i}}, \frac{\partial}{\partial x_{j}}]=0$)

19) Плоское ли $TS^{2}$?
