# Copyright 2014 Pants project contributors (see CONTRIBUTORS.md).
# Licensed under the Apache License, Version 2.0 (see LICENSE).

python_test_suite(
  name='tasks',
  dependencies=[
    ':aapt_gen',
  ],
)

python_test_suite(
  name = 'integration',
  dependencies = [
    ':dx_compile_integration',
    ':aapt_builder_integration',
    ':jarsigner_integration',
  ],
)

python_tests(
  name = 'aapt_builder_integration',
  sources = [
    'test_aapt_builder_integration.py',
  ],
  dependencies = [
    'tests/python/pants_test/android:android_integration_test',
  ],
)

python_tests(
  name='aapt_gen',
  sources=[
    'test_aapt_gen.py',
  ],
  dependencies=[
    'src/python/pants/backend/android/tasks:all',
  ],
)

python_tests(
  name = 'dx_compile_integration',
  sources = [
    'test_dx_compile_integration.py',
  ],
  dependencies = [
    'tests/python/pants_test/android:android_integration_test',
  ],
)


python_tests(
  name = 'jarsigner_integration',
  sources = [
    'test_jarsigner_integration.py',
  ],
  dependencies = [
    'tests/python/pants_test/android:android_integration_test',
    'tests/python/pants_test/tasks:base',
  ],
)
