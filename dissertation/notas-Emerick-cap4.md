## Frases tufas no livro do Emerick

- Seção 4.1, última frase do primeiro parágrafo (p. 130 do arquivo)
While parameters refer to the “static” uncertainty properties of
the reservoir, states refer to the “dynamic” variables that evolve over time,
such as pressure, temperature, phase saturation, and fluid composition.

- Seção 4.1, nota de rodapé na última frase (p. 131 do arquivo)
The attentive reader may have noticed that
we used the term “forecasting” instead of “prediction.” It appears that these words
are used interchangeably in the literature. In fact, the original Kalman filter paper by
Kalman [228] uses the word “prediction.” However, we are going to make a distinction
between the two words. We use “prediction” as a more general term; for example, we
use “prediction” for a state generated from a model. In this sense, we can use a model
to predict a past state, sometimes referred to as “hindcasting” [98]. We can also use
the model to predict the present, which is referred to as “nowcasting” [338]. We reserve
the word “forecasting” for the prediction of future states.

- Subseção 4.2.3, nota de rodapé após a equação (4.62) (p. 146 do arquivo)
It is worth noting that the first-order Markov condition holds in reservoir simulations,
where the state (say, pressure and saturation) at time tn is solely dependent on static
parameters and the state at the preceding time step, tn−1. This property is precisely
why we can employ restarts in reservoir simulators.

- Subseção 4.2.3, primeira frase após a figura 4.4 -> assimilação simultânea = sequencial ! (p. 146 do arquivo)
SDA fits in the Bayesian framework as illustrated in Fig. 4.4, which de-
picts the main elements. In this process, sequential and simultaneous data
assimilation are equivalent.

- Pseudo-código 4.2: versão bayesiana do filtro de Kalman (p. 148 do arquivo)
1. Forecast: apply the forward model to obtain the PDF of the state
at time tn given the observations up to time tn−1
2. Analysis: update the PDF using Bayes’ rule

- Seção 4.3, última frase do primeiro parágrafo (p. 149 do arquivo) 
For example, contemporary reservoir models consist
of O($10^6$) gridblocks, resulting in a $C_y$ matrix with a staggering O($10^{12}$)
entries, which is impractical to store in memory.

- Subseção 4.3.5 (p. 162-163 do arquivo)
Filter divergence occurs when the EnKF estimates deviate significantly from
the true state, as illustrated in Fig. 4.10. Once filter divergence takes hold,
it becomes an irreversible situation, and the EnKF is no longer capable of
correcting the estimates to converge with the true state. This divergence
phenomenon typically arises due to a gradual underestimation of the state
covariance, leading to a scenario where $C^f_{dd^n} \ll C_{e^n}$ [59], 
causing the filter to begin missing observations. 
Several factors contribute to filter divergence, including inadequate parametrization, model errors, incorrect (underestimated) specification of the data error covariance Ce, sampling errors,
and limitations in degrees of freedom due to the small size of the ensemble.

- Seção 5.1, segundo parágrafo (p.166 do arquivo)
One alternative to the EnKF is the ensemble smoother (ES) [448, 400]. In
ES, all data are assimilated simultaneously in a single update, eliminating
the need for simulation restarts. However, the single update scheme of ES
has proven insufficient for properly conditioning reservoir models to dynamic
data [77, 132, 133]. This limitation has driven the development of iterative
forms of ES [77, 78, 132, 413, 279, 354].

- Seção 7.5, primeiro parágrafo (p. 233) do arquivo
Localization [197] is another ad hoc procedure employed to mitigate the
negative effects of small ensembles. Typically, localization assumes that the
covariances between model parameters and data are a function of distance.
In its simplest form, localization aims to restrict the influence of a component of the innovation vector (data mismatch term) to a region around the
data location. Localization is highly effective, simple to implement, and computationally inexpensive. 
However, determining the appropriate localization region depends on the specific problem.

- Seção 7.5.3, primeiro parágrafo (p. 227 do arquivo)
In distance-based localization, the localization matrix Rmd used in the Schur
product is computed based on the distance between model parameters and
observation locations. Essentially, the localization coefficients assign weights
to covariance values based on their spatial separation: closer points receive
higher weights, while distant points receive lower weights.

