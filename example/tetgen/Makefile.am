
# This file is part of p4est.
# Makefile.am in example/tetgen
# included non-recursively from toplevel directory

dist_p4estdata_DATA += \
        example/tetgen/p8est_box_tetgen.ele \
        example/tetgen/p8est_box_tetgen.node

if P4EST_ENABLE_BUILD_2D
bin_PROGRAMS += example/tetgen/p4est_read_conn
example_tetgen_p4est_read_conn_SOURCES = example/tetgen/read_conn2.c

LINT_CSOURCES += $(example_tetgen_p4est_read_conn_SOURCES)
endif

if P4EST_ENABLE_BUILD_3D
bin_PROGRAMS += example/tetgen/p8est_read_tetgen example/tetgen/p8est_read_conn
example_tetgen_p8est_read_tetgen_SOURCES = example/tetgen/read_tetgen.c
example_tetgen_p8est_read_conn_SOURCES = example/tetgen/read_conn3.c

LINT_CSOURCES += $(example_tetgen_p8est_read_tetgen_SOURCES) \
                 $(example_tetgen_p8est_read_conn_SOURCES)
endif
