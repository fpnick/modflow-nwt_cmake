cmake_minimum_required (VERSION 2.6)
project (MODFLOW-NWT)
enable_language( Fortran )
set( Toolchain gFortran )

file(GLOB mfnwt_src "*.f" "*.f90" )

add_executable(mfnwt ${mfnwt_src})

SET_TARGET_PROPERTIES(mfnwt PROPERTIES LINKER_LANGUAGE Fortran)
