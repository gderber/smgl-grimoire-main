mkdir  buildit &&
cd     buildit &&

../configure  --host=$HOST                  \
              --build=$BUILD                \
              --prefix=/usr                 \
              --infodir=${TRACK_ROOT}/usr/share/info     \
              --mandir=${TRACK_ROOT}/usr/share/man       \
              --enable-shared               \
              --disable-static              \
              --disable-werror              \
              --enable-ld=default           \
              --enable-gold                 \
              $OPTS  &&
make DESTDIR=$INSTALL_ROOT
