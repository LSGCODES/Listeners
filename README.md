# Eventos

### Criando a classe e a registrando
### Listeners
Um listener é uma classe que monitora os eventos que ocorrem na API Bukkit, como a ação de quebrar blocos, ou simplesmente eventos de outros plugins. 
### Suporte ??
Caso tenha alguma dúvida em relação ao código, entre em contacto comigo. https://discord.gg/BaBnxGME2X
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
