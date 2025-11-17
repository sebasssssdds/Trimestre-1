# funcion para establecer conexion wifi

def do_connect(SSID, PASSWORD):
  import network
  global sta_if
  sta_if = network.WLAN(network.STA_IF)
  if not sta_if.isconnected():
      sta_if.active(True)
      sta_if.connect(SSID, PASSWORD)
      print('Conectada a la red', SSID + "...")
      while not sta_if.isconnected():
          pass
      print('Configuracion de la red (IP/netmask/gw/DNS):', sta_if.ifconfig())

do_connect('clasee1', '12345678')
  
