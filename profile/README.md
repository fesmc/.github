<h1 align="center">Fast Earth System Model Community</h1>

<p align="center">
  <b>Learn from the past. Project the future.</b>
</p>

We build Earth system models that are fast enough to simulate the deep past. Our tools are used to study timescales from decades to glacial–interglacial cycles, with a strong focus on ice sheets and the systems they interact with.

| 🧊 Model the past | 🔍 Gain insight | 🔭 Project the future |
|---|---|---|
| Run long paleoclimate simulations and many ensemble members, and compare them with the geological record. | Switch processes and feedbacks on and off to find out what drives the changes we see. | Apply what we learn to projections, from the coming decades to many millennia. |

fesmc is an open community for sharing the tools that make this possible. We develop them along **two main lines**, one in **Julia** and one in **Fortran**.

---

## 🟣 Julia: a new generation of models

Our Julia packages explore what modern tools can bring to fast modelling, such as GPU execution and automatic differentiation. Three of them have **model description papers in preparation**:

| Model | What it does | Links |
|---|---|---|
| **[Laddie.jl](https://github.com/fesmc/Laddie.jl)** | **Basal melt beneath Antarctic ice shelves.** A differentiable implementation of the one-layer ocean model [LADDIE](https://doi.org/10.5194/tc-17-3203-2023) (Lambert et al., 2023) that runs on CPUs and GPUs. | [Docs](https://fesmc.github.io/Laddie.jl/dev/) |
| **[Chion.jl](https://github.com/fesmc/Chion.jl)** | **Snowpack and firn** for ice sheets and seasonal snow. Computes the surface mass and energy balance on CPUs and GPUs, with a choice of multilayer, positive-degree-day and insolation–temperature–melt models. | [Docs](https://fesmc.github.io/Chion.jl/dev/) |
| **[FastHydrology.jl](https://github.com/fesmc/FastHydrology.jl)** | **Subglacial hydrology.** Computes the effective pressure at the ice base, which links subglacial water to basal sliding, with models designed for coupling to ice-flow models. | [Docs](https://takisangelides.github.io/FastHydrology.jl/dev/) |

---

## 🟠 Fortran: established models for science

Our Fortran line includes two models that are already **widely used in the scientific literature**.

### [CLIMBER-X](https://github.com/cxesmc/climber-x): fast Earth system model

CLIMBER-X simulates the evolution of the Earth system on timescales from decades to glacial–interglacial cycles. It brings together atmosphere, ocean, sea ice, land, carbon cycle, ice sheets and solid Earth. Most components are open source, while access to some is still restricted.

[Code](https://github.com/cxesmc/climber-x) · [Docs](https://cxesmc.github.io/climber-x/) · Description papers: [climate](https://doi.org/10.5194/gmd-15-5905-2022), [carbon cycle](https://doi.org/10.5194/gmd-16-3501-2023)

### [Yelmo](https://github.com/fesmc/yelmo): ice-sheet model

Yelmo is a 3D ice-sheet–shelf model that solves the coupled dynamics and thermodynamics of ice sheets. It can be run in idealized setups, as a stand-alone ice-sheet model or coupled to climate, and it is one of the ice-sheet components of CLIMBER-X. For realistic regional simulations, start with [YelmoX](https://github.com/fesmc/yelmox).

[Code](https://github.com/fesmc/yelmo) · [Docs](https://fesmc.github.io/yelmo/) · [Description paper](https://doi.org/10.5194/gmd-13-2805-2020)

**Also in Fortran:** [FastHydrology](https://github.com/fesmc/FastHydrology) (basal hydrology) · [chion](https://github.com/fesmc/chion) (snowpack) · [insol](https://github.com/fesmc/insol) (paleo and future insolation) · [fesm-utils](https://github.com/fesmc/fesm-utils) (shared libraries)

---

## 🤝 Get involved

Try a model, open an issue or send a pull request in the relevant repository. You can also browse [all our repositories](https://github.com/orgs/fesmc/repositories). If you use one of our models in your work, please cite it as described in its repository or documentation.
