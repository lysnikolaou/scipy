py3.extension_module('_rotation',
  [cython_gen.process('_rotation.pyx')],
  c_args: [cython_c_args, Wno_maybe_uninitialized],
  dependencies: np_dep,
  link_args: version_link_args,
  install: true,
  subdir: 'scipy/spatial/transform'
)

py3.extension_module('_rigid_transform_cy',
  [cython_gen.process('_rigid_transform_cy.pyx')],
  c_args: [cython_c_args, Wno_maybe_uninitialized],
  dependencies: np_dep,
  link_args: version_link_args,
  install: true,
  subdir: 'scipy/spatial/transform'
)

py3.install_sources([
    '__init__.py',
    '_rigid_transform.py',
    '_rotation_groups.py',
    '_rotation_spline.py',
    'rotation.py'
  ],
  subdir: 'scipy/spatial/transform'
)

subdir('tests')
