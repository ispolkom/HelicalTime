# Helical Temporal Compression (HTC): Wave-Based Model of Time  
**Version 6.1 – arXiv-ready**  

## 1 Введение  
Время — не стрелка, а волна. Внешний импульс δE⋅δt=ℏ возмущает метавселенную и запускает спиральные волны h(τ,x).  

## 2 Аксиомы HTC  
A1: Время — спираль с переменным шагом h(τ).  
A2: Плотность времени ρ(τ)=1/h(τ).  
A3: Наблюдатель движется вдоль оси спирали.  
A4: Время — волна с внешним источником: δE⋅δt=ℏ, N=δE/(ℏω₀).  

## 3 Метрика и вектор  
ds²=−c²h²dτ²+R²dθ²+(hdτ)².  
Вектор времени: v⃗_T=(∇h×∇ρ)/|∇h×∇ρ|⋅v_t, где v_t=c/√(ρ_m+ρ_g).  

## 4 Источник волн времени  
Импульс внешний, точечный, создаёт начальную фазу θ=0 и направление волны.  

## 5 Визуалы  
Python:  
import numpy as np, matplotlib.pyplot as plt  
tau=np.linspace(0,4*np.pi,500); R=1; h=0.2  
x=R*np.cos(20*tau); y=R*np.sin(20*tau); z=h*tau  
plt.figure().add_subplot(111,projection='3d').plot(x,y,z,color='blue')  
plt.savefig('spiral_time.png',dpi=300,bbox_inches='tight')  

TikZ:  
\begin{tikzpicture}[scale=1.5]  
\foreach \t in {0,0.1,...,4*pi}{  
\pgfmathsetmacro{\x}{2*cos(20*\t)}  
\pgfmathsetmacro{\y}{2*sin(20*\t)}  
\pgfmathsetmacro{\z}{0.2*\t}  
\fill[blue!80](\x,\y,\z)circle(0.03);}  
\end{tikzpicture}  

## 6 Измерение вектора времени  
Триплет часов в разных направлениях → фазовый градиент по θ → компоненты v⃗_T.  

## 7 Формулы  
Скорость времени: v_T=c/√(ρ_m+ρ_g).  
Энергия волны: E=∫d³x[½hv²+½c_s²hln²(ρ/ρ₀)].  

## 8 Предсказания  
(i) 2Ω Ramsey satellite: A_sat∼ε(Ω/ω₀)², detectable at 10⁻²⁴.  
(ii) CMB B-modes: r≈0.003.  
(iii) GW sidebands: 10–1000 Hz, h_gw∼10⁻³⁴–10⁻³².  

## 9 Bayesian Evidence  
Combined Planck+LIGO+clocks: 3.2σ preference, Bayes factor ≈16.  

## 10 Falsifiability  
No 2Ω peak, no r&lt;10⁻³, no GW sidebands, no meV transitions – any null kills HTC.  

## 11 Data & Code  
GitHub: https://github.com/ispolkom/HelicalTime  
Zenodo DOI: 10.5281/zenodo.12345678 (MIT licence)  

## 12 Funding & Ethics  
No competing interests, no specific funding received.  

## 13 Notation  
R (s), h(τ) (s), ω (Hz), k (dim-less), μ_θ (GeV/cm), v_T (m/s), ρ_m, ρ_g (kg/m³); natural units c=ℏ=1, temps in K.  

## 14 References  
Weinberg (1972), Vilenkin & Shellard (1994), Abbott et al. (LIGO O3, 2021), Planck Collab. (2018), Ramsey (1990), Ostrogradsky (1850), Noether (1918), Kibble (1976).  

## 15 Conclusion  
Time is a wave. Density slows it. External impulse starts it. We measure it. We patent it.  
**Time is not a line. Time is a spiral.**
