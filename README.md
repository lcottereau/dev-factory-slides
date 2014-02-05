Usine de développement
==================

Présentation sur les outils de dev


## Les briques de l'usine de dev

* Document : __Usine de développement__
* Présentation des outils 
 * outils de dev (maven, IDE, ...). inclure le versionning de base de données avec [Liquibase, Flyway ou autre](http://flywaydb.org/#features)
 * parler des outils de test, [évoquer Gatling en alternative à Jmeter](http://blog.xebia.fr/2013/07/11/gatling-ou-comment-ecrouler-un-serveur-alternative-a-jmeter/)
 * dépôt de code versionné : demander ce qu'ils ont retenu de l'intérêt (historique, documentation, sauvegarde, partage)
 * serveur d'intégration continue
 * dépôt de binaires (maven, rpm, ...)
 * documentation et analyse statique
 * Infrastructure avec provisionnement automatique (virtualisation, PaaS, ...)

## code Kata : [main de poker](http://codingdojo.org/cgi-bin/wiki.pl?KataPokerHands)


* Document : __description du kata_ 
* installer maven
* `mvn archetype:generate` avec options par défaut

* Document : __description git__
* `git init`
* `git add --all`
* `git commit -m "init"`
* Se connecter avec un compte `userX` à la plateforme [GitLab](http://gitlab.org/)
* Créer un projet
* `git config`
* Prendre l'URL projet en `HTTP`
* `git remote add origin http://(...)`
* `git push -u origin master`

* faire le premier ticket
* coder le test
* coder l'applicatif
* message de commit avec le numéro de ticket et FIXES (à tester)
* valider dans l'intégration continue


* mettre à jour le pom.xml

## DevOps

* [DevOps](http://techtrends.xebia.fr/#tabs-2)
 * [Infrastructure as code](http://blog.octo.com/et-si-devops-nous-emmenait-vers-tdi-test-driven-infrastructure/)
 * moins de frontière entre 2 mondes souvent pas sur les mêmes rythmes (projet, quotidien, problématiques, expertises, ...)
 * essayer de transformer le SI en self-service pour les dev, géré par les Ops (voir aussi le _cloud_, PaaS, SaaS, ...)
* préciser les principes de base de numérotation de version
* Gestion de la configuration
 * séparation binaire applicatif / configuration
 * centralisation de configuration Chef, Puppet
* Monitoring et Alerting
 * Graphite / Nagios, JmxTrans
 * LogStash, ElasticSearch, Kibana
 * Mesure de la performance
* Déploiement continu
 * Gestion des branches
 * Livraison des fonctionnalités et stratégies de déploiement
 * [Zero Downtime Deployment](http://blog.octo.com/zero-downtime-deployment/)

