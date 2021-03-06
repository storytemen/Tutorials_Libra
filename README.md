# Tutorials_Libra
Tutorials showcasing various capabilities of Libra

Working with version v4.8.1

## TOC

1. Rigid body
 * 1.1. [Construct & describe properties of rigid bodies](1_rigid_body/1_setup)

2. Integrators
 * 2.1. [Runge-Kutta 4-th order](2_integrators/1_runge_kutta_4th_order)

3. Linear Algebra
 * 3.1. [operations with VECTOR, MATRIX, and CMATRIX data types](3_linear_algebra/1_vector_matrix_cmatrix_basics)

4. Optimization
 * 4.1. [Gradient descent optimizer](4_optimization/1_gradient_descent)
 * 4.2. [line search using DIIS](4_optimization/2_diis)

5. Electronic Structure Calculations in Libra
 * 5.1. [Extended Huckel Theory, EHT](5_electronic_structure/1_eht)
    * 5.1.1. [Compact version](5_electronic_structure/1_eht/1_compact)
    * 5.1.2. [Detailed version](5_electronic_structure/1_eht/2_detailed)

 * 5.2. [Incomplete Neglect of Differential Overlap, INDO](5_electronic_structure/2_indo)
    * 5.2.1. [Compact version](5_electronic_structure/2_indo/1_compact)

6. Dynamics with Libra
 * 6.1. [Quantum-classical, trajectory methods](6_dynamics/1_trajectory_based)
   * 6.1.1. [Model, adiabatic MD](6_dynamics/1_trajectory_based/1_model_adiabatic)       
        * 6.1.1.1. [NVE ensemble](6_dynamics/1_trajectory_based/1_model_adiabatic/1_nve)
        * 6.1.1.2. [NVT ensemble](6_dynamics/1_trajectory_based/1_model_adiabatic/2_nvt)
             * 6.1.1.2.1 [1 electronic state](6_dynamics/1_trajectory_based/1_model_adiabatic/2_nvt/1_1_state)
    * 6.1.2. [Model, common approach to adiabatic, Ehrenfest, and TSH](6_dynamics/1_trajectory_based/2_model_adiabatic)
    * 6.1.3. [Model, Ehrenfest recipes](6_dynamics/1_trajectory_based/3_model_ehrenfest_recipes)

 * 6.2. [Quantum-classical, neglect-of-back-reaction trajectory workflows](6_dynamics/2_nbra_workflows)
    * 6.2.1. [step 1 with DFTB+](6_dynamics/2_nbra_workflows/1_step1_dftb)
    * 6.2.2. [step 1 with QE](6_dynamics/2_nbra_workflows/2_step1_qe)
    * 6.2.3. [step 2 with QE](6_dynamics/2_nbra_workflows/3_step2_qe)
    * 6.2.4. [step 3](6_dynamics/2_nbra_workflows/4_step3)  
      * 6.2.4.1 [build_SD_basis](6_dynamics/2_nbra_workflows/4_step3/1_build_SD_basis)    

 * 6.3. [Hierarchical equations of motion, HEOM](6_dynamics/3_heom)

 * 6.4. [DVR, on-the-grid wavepackets](6_dynamics/4_wavepackets)

 * 6.5. [Fermi Golden Rule rates, FGR](6_dynamics/5_fgr)

7. Special Functions
 * 7.1. [Sorting, matrix statistics](7_special_functions/1_sorting_matrix_statistics)


_______________________________

## Use cases

1. Create a chemical system
  * [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
  
2. EHT calculations with Libra
  * [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)

3. INDO calculations with Libra
  * [5.2.1.](5_electronic_structure/2_indo/1_compact/tutorial.ipynb)

4. Compute .cube files from orbitals computed with Libra
  * [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
  * [5.2.1.](5_electronic_structure/2_indo/1_compact/tutorial.ipynb)

5. Visualize the MOs from .cube files
  * [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
  * [5.2.1.](5_electronic_structure/2_eht/1_compact/tutorial.ipynb)

6. Compute pDOS from built-in electronic structure calculations in Libra
  * [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)

7. Plot pDOS computed with Libra
  * [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)

8. Visualize MD trajectory with py3Dmol:
  * [6.2.1.](6_dynamics/2_nbra_workflows/1_step1_dftb/tutorial.ipynb)

9. Constructing the vibronic Hamiltonian from the QE MD calculations:
  * [6.2.3.](6_dynamics/2_nbra_workflows/3_step2_qe/tutorial.ipynb)

10. Reading the vibronic Hamiltonian data files to obtain its properties:
  * [6.2.3.](6_dynamics/2_nbra_workflows/3_step2_qe/tutorial.ipynb)
  * [6.2.4.1.](6_dynamics/2_nbra_workflows/4_step2_qe/tutorial.ipynb)

11. Compute the time-averaged nonadiabatic couplings of the vibronic Hamiltonian:
  * [6.2.3.](6_dynamics/2_nbra_workflows/3_step2_qe/tutorial.ipynb)
  * [6.2.4.1.](6_dynamics/2_nbra_workflows/4_step3/build_SD_basis/tutorial.ipynb)

12. Manually construct a Slater Determinant basis:
  * [6.2.4.1.](6_dynamics/2_nbra_workflows/4_step3/build_SD_basis/tutorial.ipynb)

13. Using Libra to auto-generate a Slater Determinant basis:
  * [6.2.4.1.](6_dynamics/2_nbra_workflows/4_step3/build_SD_basis/tutorial.ipynb)

14. Compute the energies and nonadiabatic couplings in the SD basis:
  * [6.2.4.1.](6_dynamics/2_nbra_workflows/4_step3/build_SD_basis/tutorial.ipynb)

15. Calculate population and coherence dynamics of a quantum system embedded in a bath
   * [6.3.1.](6_dynamics/1_dynamics_and_lineshapes/3_heom/tutorial.ipynb)
   
16. Calculate absorbance spectral lineshapes of a quantum system embedded in a bath
   * [6.3.1.](6_dynamics/3_heom/1_dynamics_and_lineshapes/tutorial.ipynb)
_______________________________


## Functions

- `liblibra::libqm_tools`
  - `charge_density` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
  - `compute_dos` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)


- `libra_py`
  - `LoadMolecule`
    - `Load_Molecule` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
   
  - `LoadPT`
    - `Load_PT` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    
  - `pdos`
    - `libra_pdos` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)

  - `workflows`
    - `nbra`
      - `step2`
        - `run` [6.2.3.](6_dynamics/2_nbra_workflows/3_step2_qe/tutorial.ipynb)
      - `step3`
        - `build_SD_basis` [6.2.4.1.](6_dynamics/2_nbra_workflows/4_step3/build_SD_basis/tutorial.ipynb)
        - `run` [6.2.4.1.](6_dynamics/2_nbra_workflows/4_step3/build_SD_basis/tutorial.ipynb)       

  - `QE_methods`
    - `out2inp` [6.2.3.](6_dynamics/2_nbra_workflows/3_step2_qe/tutorial.ipynb)

  - `hpc_utils`
    - `distribute` [6.2.3.](6_dynamics/2_nbra_workflows/3_step2_qe/tutorial.ipynb)

  - `data_read`
    - `get_data_sets` [6.2.3.](6_dynamics/2_nbra_workflows/3_step2_qe/tutorial.ipynb)

  - `data_stat`
    - `cmat_stat2` [6.2.3.](6_dynamics/2_nbra_workflows/3_step2_qe/tutorial.ipynb)
    
  - `dynamics`
    - `heom`
      - `compute` 
        - `run_dynamics`[6.3.1.](6_dynamics/3_heom/1_dynamics_and_lineshapes/tutorial.ipynb)
        
  - `ft`
    - `ft2`[6.3.1.](6_dynamics/3_heom/1_dynamics_and_lineshapes/tutorial.ipynb)
        
_______________________________


## Classes and class members

- `liblibra::libcontrol_parameters::Control_Parameters` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)


- `liblibra::libchemobjects`
  - `libchemsys::System`
    - `Number_of_atoms` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    - `get_xyz` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
        
    
  - `libuniverse::Universe` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)


- `liblibra::libhamiltonian::libhamiltonian_atomistic::libhamiltonian_qm`
  - `listHamiltonian_QM`
    - `compute_scf` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    - `get_electronic_structure` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    - `basis_ao` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    - `atom_to_ao_map` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)


  - `Electronic_Structure`
    - `Nelec` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    - `Norb` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    - `get_bands_alp` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    - `get_bands_bet` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    - `get_occ_alp` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)
    - `get_occ_bet` [5.1.1.](5_electronic_structure/1_eht/1_compact/tutorial.ipynb)

