  cd binutils-$VERSION &&

  rm -rf buildit &&

  mkdir buildit &&
  cd buildit &&

  for TARGET in $TARGETS; do

    message "${MESSAGE_COLOR}Compiling for target : $TARGET${DEFAULT_COLOR}" &&
    PROGRAM_PREFIX=${TARGET}-           &&
    TOOLDIR=/usr/lib/${TARGET}          &&

    mkdir $TARGET                       &&
    cd $TARGET                          &&

    ../../configure                     \
      --host=$BUILD                     \
      --prefix=/usr                     \
      --program-prefix=$PROGRAM_PREFIX  \
      --target=$TARGET                  \
      $OPTS				&&

    make  tooldir=$TOOLDIR              &&
    cd ..                               
  done  

