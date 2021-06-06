# Berichte &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp;  ![git](https://www.eduopinions.com/wp-content/uploads/2018/01/fh-aachen-university-of-applied-sciences-303-logo-140x41.png)



**Bekbichi, Oussama** &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp;  &nbsp; &nbsp; &nbsp;   &nbsp; &nbsp; &nbsp;   &nbsp; **AMI**


_______________________________________________________

# Multitasking und Multithreading:
 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; ![git](https://cdn3.iconfinder.com/data/icons/web-design-development-8/24/development_design-multitasking-task-application-computer-copy-128.png)  ![git](https://api.nuget.org/v3-flatcontainer/multithreading.scheduler/3.0.0/icon)

***********************************

### Unterschied zwischen einem Prozess und einem Thread :

 -	Ein Prozess bedeutet, dass ein Programm ausgeführt wird, aber einem Thread bedeutet ein Segment eines Prozesses.
-	Ein Prozess ist nicht Lightweight, wohingegen Threads Lightweight sind.
-	Das Beenden eines Prozesses benötigt mehr Zeit als einem Thread.
-	Der Prozess benötigt mehr Zeit für die Erstellung Als einem Thread.
-	Der Prozess benötigt wahrscheinlich mehr Zeit für die Kontextumschaltung als dem Thread.
-	Ein Prozess ist größtenteils isoliert, während Threads den Speicher gemeinsam nutzen.
-	Der Prozess teilt keine Daten, aber Threads teilen Daten miteinander.

### Unterschied zwischen Multitasking und Multithreading:

| **Multitasking** | **Multithreading** |
| ------ | ------ |
|Beim Multitasking dürfen Benutzer viele Aufgaben nach CPU ausführen. | Beim Multithreading werden viele Threads aus einem Prozess erstellt, durch den die Computerleistung erhöht wird. |
| Multitasking beinhaltet häufig das Umschalten der CPU zwischen den Tasks. |Auch beim Multithreading ist häufig ein CPU-Switching zwischen den Threads beteiligt.|
| Beim Multitasking teilen sich die Prozesse einen separaten Speicher.| Beim Multithreading wird Prozessen der gleiche Speicher zugewiesen. |
|Die Multitasking-Komponente beinhaltet Multiprocessing. | Während die Multithreading-Komponente kein Multiprocessing beinhaltet. |
|Beim Multitasking wird eine CPU bereitgestellt, um viele Aufgaben gleichzeitig auszuführen.|Auch beim Multithreading wird eine CPU bereitgestellt, um viele Threads eines Prozesses gleichzeitig auszuführen.|
|Beim Multitasking teilen sich Prozesse nicht dieselben Ressourcen, jedem Prozess werden separate Ressourcen zugewiesen.|Beim Multithreading teilen sich alle Prozesse dieselben Ressourcen.|
|Multitasking ist im Vergleich zu Multithreading langsam.|Während Multithreading schneller ist.|
|Beim Multitasking dauert die Beendigung des Prozesses länger.|Beim Multithreading dauert die Beendigung des Threads weniger Zeit.|
### Kooperativ und präemptiv im Zusammenhang von Multitasking/Multithreading :
||Multitasking|Multithreading|
| ------ | ------ | ------ |
|**kooperativ**|Beim kooperativen Multitasking initiiert das Programm niemals eine Kontextumschaltung vom laufenden Prozess zu einem anderen Prozess. Ein Kontextwechsel erfolgt nur, wenn die Prozesse freiwillig regelmäßig die Kontrolle übernehmen oder wenn sie inaktiv oder logisch blockiert sind, damit mehrere Anwendungen gleichzeitig ausgeführt werden können. Außerdem arbeiten bei diesem Multitasking alle Prozesse zusammen, damit das Planungsschema funktioniert.|Beim kooperativen Multithreading wird ein Thread ausgeführt, bis er eine Methode aufruft, das zu einem anderen Thread wechselt.|
|**präemptiv**|Im präemptive Multitasking ermöglicht das Programm das Stoppen der Ausführung des laufenden Prozesses und das Zuordnen der CPU zu einem anderen Prozess. Der Mechanismus, das Betriebssystem von einem Prozess aus zu kontrollieren und einem anderen Prozess zuzuführen, wird Präempting oder Präemption genannt.|Beim präemptive Multithreading ermöglicht das Programm jederzeit von einem Thread zum anderen gehen.|


### Unterschied zwischen Distributed-Memory und Shared-Memory und die Auswirkungen für den Programmierer:


 **Shared Memory** und **Distributed Memory** sind Programmierabstraktionen auf niedriger Ebene, die bei bestimmten Arten der parallelen Programmierung verwendet werden.
![übersicht](https://img.shields.io/badge/-Shared%20Memory-red)
> Der **Shared Memory**  ermöglicht es ***_mehreren Verarbeitungselementen_***, denselben Speicherort (dh das gegenseitige Lesen und Schreiben) ohne andere spezielle Anweisungen gemeinsam zu nutzen. Als Auswirkung von **Shared Memory** können Prozesse und Threads direkt miteinander kommunizieren. Die Synchronisation des gemeinsam genutzten Speichers liegt in der Verantwortung des Anwendungsprogramms.

![übersicht](https://img.shields.io/badge/-Distributed%20Memory-red)

> **Distributed Memory** erfordert explizite Befehle zum Übertragen von Daten von einem Verarbeitungselement zu einem anderen, was als **Auswirkung** hat, dass der Programmierer Kommunikation programmieren muss.




### Nutzung der Multitasking und Multithreading:
![übersicht](https://img.shields.io/badge/-Multithreading-red)
> Man benutzt Multithreading,denn :
- es Haltet Die Programm reaktionsschnell.
-  es Nutzt CPU besser. Die CPU kann durch IO oder andere Dinge blockiert werden. 
-  Mehrere Threads können für mehrere CPU-Kerne geplant werden.
- Manche Probleme sind natürlich durch Multithreading zu lösen. Eine solche Lösung kann Ihren Code vereinfachen.

![übersicht](https://img.shields.io/badge/-Multitasking-red)
> Andererseits benutz man Multitasking, denn :
- Multitasking ist ein Prozess, bei dem mehrere Aufgaben gleichzeitig ausgeführt werden. Wir verwenden Multitasking, um die CPU zu nutzen. Multitasking kann auf zwei Arten erreicht werden:
    - Prozessbasiertes Multitasking (Multiprocessing)
    - Thread-basiertes Multitasking (Multithreading)

### Race Condition:

> Eine Race Condition ist die Bedingung, bei der das wesentliche Verhalten des Systems von der Sequenz oder dem Timing anderer unkontrollierbarer Ereignisse abhängt. Es wird zu einem Fehler, wenn eines oder mehrere der möglichen Verhaltensweisen unerwünscht sind. Eine Race Condition tritt auf, wenn zwei oder mehr Threads auf freigegebene Daten zugreifen können und gleichzeitig versuchen, diese zu ändern.

### Synchronisation im Zusammenhang von Multithreading:

> Die Synchronisierung, im Zusammenhang von Multithreading, ist ein Prozess zur Handhabung des Ressourcenzugriffs durch mehrere Thread-Anforderungen. Der Hauptzweck der Synchronisation besteht darin, Thread-Interferenzen zu vermeiden.

### Deadlock:

> Deadlock ist eine Situation, in der zwei oder mehr Prozesse aufeinander warten. Ein Deadlock tritt auf, wenn der wartende Prozess noch an einer anderen Ressource festhält, die der erste benötigt, bevor er abgeschlossen werden kann.

**Beispiel**:
_Die Ressourcen A und B werden von den Prozessen X und Y verwendet_ :

- X beginnt, A zu verwenden.
- X und Y versuchen B zu verwenden
- Y 'gewinnt' und bekommt B zuerst
- jetzt muss Y A verwenden
- A wird von X gesperrt, das auf Y wartet
- Deadlock

### Threadsicherheit (**thread safety**):

> Thread-Sicherheit oder Thread-sicherer Code bezieht sich auf Code, der sicher in einer Concurrent- oder Multi-Threading-Umgebung verwendet oder gemeinsam genutzt werden kann und sich wie erwartet verhält.

### Synchronisationsmechanismen Barrier und Semaphore :
### Barriere:
Eine Barriere für eine Gruppe von Threads oder Prozessen bedeutet, dass jeder Thread/Prozess an diesem Grenz anhalten muss und kann nicht fortgesetzt werden, bis alle anderen Threads/Prozesse diese Grenz (Barriere) erreichen.
### Semaphore:

Ein Semaphor ist ein Objekt, das die Eingabe bestimmter Ressourcen steuert. Das heißt, wenn ein Thread auf diese Ressource zugreifen möchte, muss er die Berechtigung für diesen Semaphor anfordern, der den Zugriff gewähren kann oder nicht.

--------------------------------------------------------------------
# Java &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; ![git](https://www.01net.com/images/logiciel/8138.gif) 

--------------------------------------------------------------------
### Java Multithreading Klass:
> Das Java-Multithreading-System baut auf der Thread-Klasse auf :
```
java.lang.Thread
java.lang.ThreadGroup
java.lang.Runnable
```

### Java Threads Synchronisation:
> Es gibt zwei Arten der gegenseitigen Exklusiv- und der Interthread-Kommunikation der Thread-Synchronisation.

- Gegenseitig exklusiv :
    - Synchronisierte Methode.
    + Synchronisierter Block.
    + statische Synchronisation.
    - **Beispiel**:
```java
        public  class Client {
    public  static  synchronized  int getId() {
    //code
   }
}
```
- Kooperation (Inter-Thread-Kommunikation in Java)
    - **Beispiel**:
```java
    public  class Client {
    public  static  synchronized  int getId() {
    synchronized(key) {
            key.notify();
      }
   }
}
```
### Unterschied ConcurrentHashMap und HashMap:

> HashMap ist eine leistungsstarke Datenstruktur in Java, die zum Speichern der Schlüsselpaarwerte verwendet wird. Es ordnet einen Wert dem zugehörigen Schlüssel zu. Die ConcurrentHashMap ist eine synchronisierte Auflistungsklasse.

> Die HashMap ist nicht threadsicher und kann nicht in einer Concurrent-Multithread-Umgebung verwendet werden. Im Vergleich dazu ist ConcurrentHashMap threadsicher und speziell für die Verwendung in Multithread- und Concurrent-Umgebungen entwickelt.

### Threadpool:

> Der Threadpool stellt eine Gruppe von Arbeitsthreads dar, die auf den Auftrag warten und viele Male wiederverwendet werden. Im Falle eines Thread-Pools wird eine Gruppe von Threads mit fester Größe erstellt.


 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp;   &nbsp; &nbsp; &nbsp;   &nbsp; &nbsp; &nbsp;  *06.06.2021*