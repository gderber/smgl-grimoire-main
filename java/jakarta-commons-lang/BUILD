. $SECTION_DIRECTORY/java-functions
  
set_ant_env  &&

# create build.properties
cat > $SOURCE_DIRECTORY/${SPELL#*-}/build.properties <<EOF
base.path=${SM_JAKARTA_HOME}
commons-collections.home=\${base.path}/commons-collections
commons-collections.jar=\${commons-collections.home}/commons-collections.jar
junit.jar=${SM_IBM_HOME}/lib/junit.jar
EOF

cd  ${SPELL#*-} &&
cp  LICENSE.txt ../LICENSE   &&
ant  dist
