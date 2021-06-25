# Eventos

### Criando a classe e a registrando
### Listeners
Um listener é uma classe que monitora os eventos que ocorrem na API Bukkit, como a ação de quebrar blocos, ou simplesmente eventos de outros plugins. 
```java
import org.bukkit.Bukkit;

public class Main extends JavaPlugin {

    public void onEnable() {
        System.out.println("new Join, eu dei basicamente um exemplo. Você precisa registrar a classe do evento, no caso a minha é Join")
        Bukkit.getPluginManager().registerEvents(new Join(), this);
    }
```

```java
import org.bukkit.event.Listener;

public class Evento implements Listener {
    code
}
```

Quando um jogador entrar no servidor:
```java
@EventHandler
public void onPlayerJoinEvent(PlayerJoinEvent e) {
    code
}
```

Quando um jogador desconectar do servidor:
```java
@EventHandler
public void onPlayerLeaveEvent(PlayerQuitEvent e) {
    code
}
```
Quando um jogador colocar um bloco:
```java
@EventHandler
public void onBlock(BlockPlaceEvent e) {
    code
}
```
