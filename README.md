# Settup
## Gradle
  159  cd gradle-travis-example/
  160  gradle init --type java-application
  161  mkdir java-demo
  162  cd java-demo
  163  gradle init --type java-application
  165  ./gradlew build
  166  ./gradlew tasks
  168  ./gradlew run
  169  history
## Travis CI
  170  git init
  173  git add --all
  174  git commit -m "first commit"
  175  git remote add origin https://github.com/kruehrig-tgm/gradle-travis-exmaple.git
  176  git push -u origin master
  177  git add --all
  178  git commit -m "deletion of 'gradlew files"
  179  git push -u origin master
Auf GitHub muss eine Datei .travis.yml erstellt werden. Für diese Aufgabe erhält sie folgenden Inhalt:

language: java
Es müssen außerdem im Verzeichnis java-demo auch die Files, die im Namen gradlew enthalten, gelöscht werden. Auf GitHub befindet man sich bereit in diesem Verzeichnis. Diese Vorgänge können lokal oder auf Github erledigt werden. ACHTUNG: Erledigt man alles online auf GitHub ist ein pull mit git pull im Verzeichnis lokal notwendig, um später keine Mergekonflikte zu erhalten. Erledigt man Teile lokal, so müssen diese Erledigungen mit git push gepusht werden.

  180  git pull
  182  git commit -m "deletion of 'gradlew' files"
  183  git add --all
  184  git push -u origin master
  185  history
  
# Helpful Links
Gradle Guides: https://gradle.org/guides/

Set up Gradle on your system: https://guides.gradle.org/building-java-applications/

Set up Travis CI for your java apllications: https://docs.travis-ci.com/user/getting-started
