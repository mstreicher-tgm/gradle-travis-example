# Settup
## Gradle
  cd gradle-travis-example/
  gradle init --type java-application
  mkdir java-demo
  cd java-demo
  gradle init --type java-application
  ./gradlew build
  ./gradlew tasks
  ./gradlew run
  
## Travis CI
  git init
  git add --all
  git commit -m "first commit"
  git remote add origin https://github.com/mstreicher-tgm/gradle-travis-exmaple.git
  git push -u origin master
  git add --all
  git commit -m "deletion of 'gradlew files"
  git push -u origin master
  
Auf GitHub muss eine Datei .travis.yml erstellt werden. Für diese Aufgabe erhält sie folgenden Inhalt:

language: java
Es müssen außerdem im Verzeichnis java-demo auch die Files, die im Namen gradlew enthalten, gelöscht werden. Auf GitHub befindet man sich bereit in diesem Verzeichnis. Diese Vorgänge können lokal oder auf Github erledigt werden. ACHTUNG: Erledigt man alles online auf GitHub ist ein pull mit git pull im Verzeichnis lokal notwendig, um später keine Mergekonflikte zu erhalten. Erledigt man Teile lokal, so müssen diese Erledigungen mit git push gepusht werden.

  git pull
  git commit -m "deletion of 'gradlew' files"
  git add --all
  git push -u origin master
  
# Helpful Links
Gradle Guides: https://gradle.org/guides/

Gradle: https://guides.gradle.org/building-java-applications/
Travis CI: https://docs.travis-ci.com/user/getting-started
