TP Vercel
Pour connaitre la version de vercel :
4.
Vercel -v
Créer un projet : 
‘vercel init angular’
‘ cd angular && vercel ‘
7.
vercel ls
8.
Vercel logs angular-chdoqocgi.vercel.app
9.
Vercel inspect angular-chdoqocgi.vercel.app
Permet de visualiser la structure du déploiement 
10.
Elles servent à ajouter des paramètres de configuration 
11. 
vercel env add plain DB_LOGIN production
12.
vercel env ls
13.
Les secrets sont des variables chiffrées qui permettent de transmettre des informations de manière sécurisé. 
14.
15.
vercel secret add my2ndSecret this_is_the_2nd_secret
vercel env add secret prod_secret production
16.
Production / preview / dev
L’environnement sert de bac a sable ou de banc de test, il permet de tester son code sans endommager l’actuel, le preview donne une idée du rendu et le prod sert, une fois les modifications ajoutées, servira de version final qui sera alors disponible pour le ‘’public’’.  
17.
18.

19. 
Un pull-request comme son nom l’indique est une demande de la part d’un élément extérieur à la branche principale dans le pub de modifier la branche vers laquelle cette requête est effectué. Cette requête est censée modifier des éléments (ajout, suppression…). Elle peut être accepté ou refuser et si elle est accepté et que certains élément rentre en conflit, il sera demandé à l’utilisateur référent de choisir si il veut conserver les éléments actuel ou les remplacer par les éléments de la requête.
20. 
Vercel effectue ici la fusion des éléments de la branche de dev et la branche master, pour reprendre le paragraphe du dessus, il accepte la fusion. 
21.
Master = production
L’intérêt est de proposer une modification du projet principal sans le changer directement. Cela permettra par exemple au chef de projet de traiter les modifications ou option ajoutées par ses développeurs les une après les autres de manières structurer.
Workflow : 
1)	Ajustement des modifications sur la branche de dev 
2)	Commit et push sur la branche dev lorsque le programme est écrit 
3)	Création d’un pull-request de cette branche faire la branche principale (master)
4)	Récupération du projet principal 

22. 
