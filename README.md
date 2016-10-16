# 0036491704

# Pitanje 1:
U bin/Debug folderu, nakon sto sam dodala ClassLibrary1 kao refernecu, pojavio se ClassLibrary1.dll i ClassLibrary1.pdb.
Kada maknem .dll file projketa class library iz foldera, referenca nestaje i program se ne moze izvrsiti jer zadana referenca nije nadjena.
Kada bih Vam slala aplikaciju, uz aplikaciju morala bih jos poslati samo .dll projekta class library.

# Pitanje 2:
Ispisat ce se stari string. Razlog tome je to što je library samo eksterni dio koda na koji se mi referenciramo, ako promijenimo nesto, a ne compileamo, ostaje referenca na stari kod, iako je napisan novi.

# Pitanje 3:
Ako pokrenemo aplikaciju s referencom na PeroClassLibrary.dll, ispisati ce se "Pero:Hello World!".

# Pitanje 4:
Kod sadržaja Bin/Debug foldera konzolne aplikacije, nakon što sam dodala pero
class library kao referencu, primjecujem PeroClassLibrary.dll file u njemu.

# Pitanje 5:
Ako obrišem originalni .dll na disku (onaj koji sam odabrala putem browse opcije) aplikacija radi zato što se takav isti .dll nalazi u bin/Debug folderu. Build i dalje radi, PeroClassLibrary se sada traži u bin/Debug folderu.

# Pitanje 6:
Kada pobrišem NodaTime direktorij unutar packages direktorija u solutionu, te buildam aplikaciju,
build proces je uspio. Zbog sadržaja packages.config svi paketi su se skinuli(NodaTime).

