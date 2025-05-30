## Co-design at UniSQ 👋

__Tools for co-design developed by UniSQ and collaborators (under construction)__

### Key Info
- This organsation holds re-usable and generic repos and packages used in the development of co-design and MDO toolchains.
- It is currently administered by Ingo Jahn and Andy Lock,
- It is __not__ the place for spefic case studies and co-design implementations. Completed and verified examples, which may be of use to new members, may be stored after discussion with Ingo and Andy

#### Development principles
- Various elements in the toolchain should interface with Python APIs. Where different launagues are required (bash/C++), ideally they have a Python API wrapper.
- Pip packages are preferred. They can be installed in editable form (`pip install -e <REPO>`) for development
- Avoid large branches which diverge significantly from the `main` branch. Merge frequently with each new feature to maintain capability.
- Try and include test modules for key features. We are typically poor at this, but it will be beneficial for a large and complex toolchain.

### Key Repos

#### `hyperVehicle`
Parameter-based geometry generation and differentation

#### `hyperPanel`
Fast and efficient approximate panel method for hypersonic aerodynamics and surface flow properties

#### `hyperGrad`
Flow-solution-agnostic aerodynamic sensitivities using efficinet panel method derivatives

#### `hyPyCFD`
Python wrappers for automated hypersonic CFD simulations 

#### 'hyperTherm'
Differentiable heat transfer and reduced-order thermal models for hypersonic vehicles

#### 'smTools`
Data-agnostic surrogate modelling tools (i.e. aerodeck surface fitting)

#### `hyperDynamics`
Common classes and functions for creating and transcribing hypersonic flight dynamics suitable for optimcal control solutions

#### `cdTools`
A selection of tools for constructing, running, and analysing co-design simulations.

## Publication List
- Lock, A., Oberman, G., Jahn, I. H., van der Heide, C., Bone, V., Dower, P. M., & Manzie, C. (2025). Hypersonic glide vehicle shape and trajectory co-design. In AIAA SCITECH 2025 Forum (p. 1337).
- Jahn, I. H. (2025). Approximate surface pressures and heat load gradients for the optimisation of hypersonic vehicles. In AIAA SCITECH 2025 Forum (p. 0952).
- van der Heide, C., Lock, A., Bone, V., Mackle, K., Jahn, I. H., Dower, P. M., & Manzie, C. (2025). Multi-mission codesign of a hypersonic vehicle leading edge with heat flux constraints. In AIAA SCITECH 2025 Forum (p. 0955).
- Mackle, K., Lock, A., Jahn, I., & van der Heide, C. (2024). Developing a co-design framework for hypersonic vehicle aerodynamics and trajectory. In AIAA SCITECH 2024 Forum (p. 0238).
- Mackle, K., & Jahn, I. (2024). Efficient and flexible methodology for the aerodynamic shape optimization of hypersonic vehicle concepts in a high-dimensional design space. In AIAA SCITECH 2024 Forum (p. 2838).
- Mackle, K. (2024). Co-design of hypersonic vehicle shape and trajectory.
- Mackle, K., & Jahn, I. (2022). Co-designing hypersonic vehicle geometry and trajectory. In 23rd Australasian Fluid Mechanics Conference–23AFMC (pp. 1-8).
- Mackle, K., Jahn, I., & Gollan, R. (2021). Understanding the impacts of aerodynamic uncertainty on optimal trajectories for hypersonic vehicles. In AIAA AVIATION 2021 FORUM (p. 2507).

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
