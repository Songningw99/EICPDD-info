# Modification of WRF codes

The modification is based on WRF-v4.4.1. Several extra output variables are added under the nwp_diagnostics outputs. 

Extra variables:
1. UP_HELI_MAX_02: Maximum updraft helicity for the 0-2 km layer.
2. ZETA_MAX_1: Maximum vertical vorticity at k=1 model level.
3. WSPD_MAX_1: Maximum wind speed at k=1 model level.

Modified scripts:
1. Registry/Registry.EM_COMMON
2. dyn_em/module_first_rk_step_part2.F
3. dyn_em/module_diffusion_em.F 
4. phys/module_diagnostics_driver.F 
5. phys/module_diag_nwp.F

WRF needs to be recompiled after such scripts are modified. 
