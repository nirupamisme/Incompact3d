# Wind-Turbine: NREL
set(case "Wind-Turbine-two-turbines")
set(example_files "")
list(APPEND example_files "adios2_config.xml")
list(APPEND example_files "input.i3d")
list(APPEND example_files "BT2_1.turb")
list(APPEND example_files "BT2_2.turb")
list(APPEND example_files "Blade_N52.al")
list(APPEND example_files "Tower.al")
AddExample("${examples_dir}" "${case}" "${example_files}")
add_subdirectory(Airfoils)
