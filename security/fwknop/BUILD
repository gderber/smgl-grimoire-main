OPTS="$FWKNOP_OPTS $OPTS" &&

make_single &&
default_build &&
make_normal &&

if is_depends_enabled $SPELL perl; then
  cd perl/FKO &&
  default_build_perl &&
  cd ../..
fi &&

if is_depends_enabled $SPELL python; then
  cd python &&
  default_build_python &&
  cd ..
fi
