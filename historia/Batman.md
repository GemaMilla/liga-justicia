# Batman

'Hora Primera Partida' = (Select min(horMsg) FROM RH_DCFREFHYDPARAGR PAR Where PAR.RefHyd= A.refhyd AND PAR.SecCnf = A.SecCnf),
'Hora Ultima Partida' = (Select max(horMsg) FROM RH_DCFREFHYDPARAGR PAR Where PAR.RefHyd= A.refhyd AND PAR.SecCnf = A.SecCnf),
'Numero de Orden' = (Select max(OrdMer) FROM RH_DCFREFHYDPARAGR PAR Where PAR.RefHyd= A.refhyd AND PAR.SecCnf = A.SecCnf),
'Numero Ejecucucion' = (Select max(NumNeg) FROM RH_DCFREFHYDPARAGR PAR Where PAR.RefHyd= A.refhyd AND PAR.SecCnf = A.SecCnf),
'Contador Numero de Ordenes' = (Select count(Distinct OrdMer) FROM RH_DCFREFHYDPARAGR PAR Where PAR.RefHyd= A.refhyd AND PAR.SecCnf = A.SecCnf),
'Contador Numero de Ejecuciones' = (Select count(Distinct NumNeg) FROM RH_DCFREFHYDPARAGR PAR Where PAR.RefHyd= A.refhyd AND PAR.SecCnf = A.SecCnf),
