# Co-design at UniSQ 🚀

_Tools for co-design developed by UniSQ and collaborators (under construction)_

### Key Info
- This organisation holds re-usable and generic repos and packages used in the development of co-design and MDO toolchains.
- It is _not_ the place for spefic case studies and co-design implementations.
  Completed and verified examples, which may be of use to new members, may be stored after discussion with Ingo and Andy
- It is currently administered by Ingo Jahn and Andy Lock.

#### Development principles
- Pease ensure Python code is formatted per PEP8. This isn't hard - tools like [Black](https://github.com/psf/black) make a lot of this a one-line command.
- Repos should be structured as `pip` packages with relevant dependencies (unless not possible), and installed as editable (`pip install -e path/to/repo`).
  Please clearly state any other system dependencies with suggested install commands.
- Avoid large branches which diverge significantly from the main branch. Merge frequently with each new feature to maintain capability.
- Try and include test modules for key features. We are typically poor at this, but it will be beneficial for a large and complex toolchain.
- Any breaking changes which affect existing APIs should be clearly communicated with the group.
- Err on side of low level functions, expecting the user to call multiple functions to perform a task. This provides flexibility and modularity to the code.
- Use of GitHub issues and discussion on individual repos is encouraged. It provides a record of discussion and changes for everyone in the co-design group.
- Angles should be in radians unless otherwise explicitly stated (variable names appended _deg).

#### Discussion points
- Should the aerodynamic repos (panel method, CFD, and gradients) be combined into a single repo? Pros: simplicity when coding. Cons: Requires more strict git workflow adherence to prevent merge conflicts. Leaning towards multiple smaller repos as we are not git masters.


## Overview of Design Tools
Design tools under developemnt have been separated into 5 groups based on the their purpose and functionality.
Boxes marked by dashed (- - ) lines are tools currently under development.
<img src="./Design Tools.svg">


# Key Repos
Refer to progress checkmarks for status of different tools and modules.


## hyperVehicle
[`hyperVehicle`](https://github.com/codesign-at-unisq/hypervehicle2)

_Parameter-based geometry generation and differentiation_

Owners: Ingo + Bradley
- [x] Import from previous organisation
- [ ] Simplify user interface
- [ ] Create documentation
- [ ] Expand capabilities to include multi-comonent vehicles.


## hyperPanel
_Fast and efficient approximate panel method for hypersonic aerodynamics and surface flow properties_

Owners: Bradley + Robert
- [ ] Seperate form old `PySAGAS` package and provide minimal documentation
- [ ] Create documentation


## hyperGrad
_Flow-solution-agnostic aerodynamic sensitivities using efficient panel method derivatives_

Owners: Amir + Ingo
- [ ] Seperate form old `PySAGAS` package and provide minimal documentation
- [ ] Create documentation


### hyPyCFD
_Python wrappers for automated hypersonic CFD simulations_

Owner: Rob
- [ ] Create minimal working repo
- [ ] Create documentation


## hyperTherm
_Differentiable heat transfer and reduced-order thermal models for hypersonic vehicles_

Owner: Saurav
- [ ] Crate minimal working repo
- [ ] Create documentation


## hyperPro
_Propulsion models for hypersonic vehicles - both air-breathing and non air-breathing._

Owners: Amir
- [ ] Crate minimal working repo
- [ ] Create documentation


## smTools
_Data-agnostic surrogate modelling tools (i.e. aerodeck surface fitting)_

Owners: Andy + Ingo
- [ ] Tidy and import from Andy's previous repo
- [ ] Wrap in `pip` package


## hyperDynamics
_Common classes and functions for creating and transcribing hypersonic flight dynamics suitable for optimal control solutions using [CasADi](https://web.casadi.org/)_

Owners: Andy + Jack
- [ ] Tidy and import from Andy's previous repo
- [ ] Create documentation


## codesigndTools
_A selection of tools for constructing, running, and analysing co-design simulations_

Owner: All co-design group
- [ ] Tidy and import from Andy's previous repo
- [ ] Wrap in `pip` package
- [ ] Create documentation


## Examples & Tests
_Selection of examples and test cases to demonstrate and verify the co-design simulations_

Owner: Ingo
- [ ] Crate minimal working repo
- [ ] Create automated test routines


# Publication List

### 2025
- Lock, A., Oberman, G., Jahn, I. H., van der Heide, C., Bone, V., Dower, P. M., & Manzie, C. (2025). Hypersonic glide vehicle shape and trajectory co-design. In AIAA SCITECH 2025 Forum (p. 1337).
- Jahn, I. H. (2025). Approximate surface pressures and heat load gradients for the optimisation of hypersonic vehicles. In AIAA SCITECH 2025 Forum (p. 0952).
- van der Heide, C., Lock, A., Bone, V., Mackle, K., Jahn, I. H., Dower, P. M., & Manzie, C. (2025). Multi-mission codesign of a hypersonic vehicle leading edge with heat flux constraints. In AIAA SCITECH 2025 Forum (p. 0955).
- Mackle, K., Lock, A., Jahn, I., & van der Heide, C. (2024). Developing a co-design framework for hypersonic vehicle aerodynamics and trajectory. In AIAA SCITECH 2024 Forum (p. 0238).

### 2024
- Mackle, K., & Jahn, I. (2024). Efficient and flexible methodology for the aerodynamic shape optimization of hypersonic vehicle concepts in a high-dimensional design space. In AIAA SCITECH 2024 Forum (p. 2838).
- Mackle, K. (2024). Co-design of hypersonic vehicle shape and trajectory.
- Mackle, K., & Jahn, I. (2022). Co-designing hypersonic vehicle geometry and trajectory. In 23rd Australasian Fluid Mechanics Conference–23AFMC (pp. 1-8).
- Mackle, K., Jahn, I., & Gollan, R. (2021). Understanding the impacts of aerodynamic uncertainty on optimal trajectories for hypersonic vehicles. In AIAA AVIATION 2021 FORUM (p. 2507).


# Contributioms
How can you contribute?
- use the code and tools, and give us feedback on results.
- give feedback on the documentation.
- contribute source code.


<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
