# turn off docmfp support (broken atm)
sedit '/\\usepackage{docmfp}/d'                         $SPELL.dtx  &&
sedit 's/^%%%%%% \\providecommand/\\providecommand/'    $SPELL.dtx  &&

latex $SPELL.ins                                                    &&

latex  --interaction batchmode  $SPELL.dtx                          &&
latex  --interaction batchmode  $SPELL.dtx                          &&
makeindex -s gind.ist $SPELL                                        &&
latex  --interaction batchmode  $SPELL.dtx                          &&
latex  --interaction batchmode  $SPELL.dtx
