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

Берем первое, второе и третье тождества, вычитаем из первого второе и и к результату прибавляем третье.
ОК, пусть то, что стоит слева, будет $l.h.s.$

$$l.h.s. = \langle \nabla_{X}{Y}, Z \rangle + \langle Y, \nabla_{X}{Z} \rangle - \langle \nabla_{Z}{X}, Y \rangle - \langle X, \nabla_{Z}{Y} \rangle + \langle \nabla_{Y}{Z}, X \rangle + \langle Z, \nabla_{Y}{X} \rangle = \langle [X, Z], Y \rangle + \langle [X, Z], Y \rangle + \langle \nabla_{X}{Y}, Z \rangle + \langle Z, \nabla_{Y}{X} \rangle$$
Теперь прибавляем и к левой, и к правой части $\langle \nabla_{X}{Y}, Z \rangle$.
Тогда справа будет стоять
$$2 \langle \nabla_{X}{Y}, Z \rangle - \langle Z, [X, Y] \rangle + \langle X, [Y, Z] \rangle + \langle Y, [X, Z] \rangle $$

11) Пусть $\Omega$ -- форма кривизны, а $\omega$ -- локальная 1-форма связности.

Я умею доказывать следующее утверждение:
*Утверждение*
Пусть $\theta \in \Omega^{k}(U, E)$ (тут $E \rightarrow M$ -- расслоение, а $U$ -- тривиализующая окрестность). 
Тогда $\nabla^{2}{\theta} = F \wedge \theta$, где $F$ -- 2-форма с значениями в эндоморфизмах $E$. Локально $F = d \omega + \omega \wedge \omega$

*Доказательство*: В тривиализующей окрестности $\nabla = d + \omega$, тогда $\nabla \theta = d \theta + \omega \wedge \theta$. Тогда $$\nabla^{2}{\theta} = (d+\omega)(d \theta + \omega \wedge \theta) = d^{2} \theta + d \omega \wedge \theta - \omega \wedge d \theta + \omega \wedge d \theta + \omega \wedge \omega \wedge \theta = d \omega \wedge \theta + \omega \wedge \omega \wedge \theta$$, т.е. если $F = d \omega + \omega \wedge \omega$, то $\nabla^{2}{\theta} = F \wedge \theta$

Локально доказано -- в общем случае, следует воспользоваться тем, что при заменах базиса $F$ склеивается в глобальную 2-форму с значениями в эндоморфизмах слоя.

Заметим, что если $T$ -- замена базиса в сечениях касательного расслоения, то локальная форма связности преобразовывается по формуле $\hat{\omega} = T^{-1} \cdot \omega \cdot T + T^{-1} \cdot dT$
(действительно, т.к. пусть $\{e_{i} \}$ -- базис в сечениях, а $\{\hat{e_{i}} \}$ -- новый базис в сечениях с матрицей перехода $T$, тогда с одной стороны $\nabla \hat{e_{i}} = e_{i} T$, а с другой по формуле Лейбница $\nabla \hat{e_{i}} = \nabla(e_{i}T) = \nabla e_{i} \cdot T + e_{i} \cdot dT = e_{i} G \cdot T + e_{i} \cdot dT = \hat{e_{i}}(T^{-1} \cdot G \cdot T + T^{-1} \cdot dT)$, где $\nabla e = e G$.)
Ну а раз так, то прямым вычислением получаем, что $F = d \omega + \omega \wedge \omega$ преобразуется при заменах базиса в сечениях по правилу $\hat{F} = T^{-1}FT$, т.е. это корректно определенная глобальная 2-форма с значениями в эндоморфизмах.

Теперь осталось вспомнить, что задать склеивающие коциклы в тривиализации $< = >$ задать правило замены координат в пространстве локальных сечений, тем самым, доказываем утверждение.

(почему в условиях стоит минус, а тут плюс -- а это без разницы, т.к. основное -- это то, что пространство связностей в расслоении есть аффинное пространство, ассоциированным пространством которого является пространство 1-форм с значениями в эндоморфизмах, поэтому $\nabla = d + w$, но ничего не мешает поставить знак $-$, например.

(18) $S^{3} \rightarrow S^{2}$ -- расслоение Хопфа.

Пусть $\mathbb{R}^{4} = \mathbb{C}^{2}$, а $\mathbb{R}^{3} = \mathbb{C} \times \mathbb{R}$, где отождествления такие:
$(x_{1}, x_{2}, x_{3}, x_{4}) <-> (z_{0}, z_{1}) = (x_{1} + i x_{2}, x_{3} + i x_{4})$
и $(x_{1}, x_{2}, x_{3}) = (z, x) = (x_{1}+ix_{2}, x_{3})$.

(потом как-нибудь)

(10)
Иными словам надо показать, что форма кривизны кососимметрична.

Можно сказать, что форма кривизны принимает значения в структурной группе расслоения, а т.к. если расслоение вещественное, то его структурная группа с $GL(n)$ редуцируется до $O(n)$, тогда алгебра Ли $\mathcal{o}(n)$ состоит в точности из всех кососимметрических матриц.

Можно еще так:




<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEzNTM0Mzc0MjFdfQ==
-->