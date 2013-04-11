La vie est pleine de promess nous en faisons tous les jours. Prenons par exemple ken et barbie:

  ken = new PerfectMan()
  barbie = new PerfectWoman()

Les deux sont parfaits et maintenant voyons comment ses deux personnes vont intéragir. 

  ken.marrie(barbie)

Ok c'est pas mal mais il se passe quoi aprés ? et bien dans les films ça s'arrête là, mais dans le monde réel ça continue.

  ken.marrie(barbie)
    .then => ken.find(job)
    .then => child = Sexe(ken, barbie)
    .then (child) => ken.takeCare(child); barbie.takeCare(child)
    .then => ken.die()
    .then => barbie.die()

Et voilà une vie parfaite terminé. Mais tout ne se réalise pas toujours comme on le souhaite, et les promesses que l'on fait ne sont pas toujours tenues. 

  ted = new Man()
  robin = new Woman()

Prenons le cas de  
