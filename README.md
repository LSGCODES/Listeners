# Eventos

### Criando a classe e a registrando
### Listeners
Um listener é uma classe que monitora os eventos que ocorrem na API Bukkit, como a ação de quebrar blocos, ou simplesmente eventos de outros plugins. 
```java
public void onEnable() {
  System.out.println("new Join, você vai registrar a classe onde está o evento. Eu dei um exemplo de Join, mas sua classe pode se outra");
  Bukkit.getPluginManager().registerEvents(new Join(), this);
```
```java
import org.bukkit.event.Listener;

public class Evento implements Listener {
}
```

Quando um jogador entrar no servidor:
```java
@EventHandler
public void onPlayerJoinEvent(PlayerJoinEvent e) {
}
```

Quando um jogador desconectar do servidor:
```java
@EventHandler
public void onPlayerLeaveEvent(PlayerQuitEvent e) {
}
```
Quando um jogador colocar um bloco:
```java
@EventHandler
public void onBlock(BlockPlaceEvent e) {
}
```
