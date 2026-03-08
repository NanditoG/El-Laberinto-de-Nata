# El-Laberinto-de-Nata
import pygame
import random
import sys
import math

pygame.init()
pygame.mixer.init()

pygame.mixer.music.load("Nivel Oculto.mp3")
pygame.mixer.music.play(-1) 

ANCHO = 900
ALTO = 600

pantalla_completa = false
pantalla = pygame.display.set_mode ((ANCHO, ALTO))
pygame.display.set_camption ("El Laberinto de Nata")

clock = pygame.time.clock()

#--------------------------
#  MAPAS
#---------------------------

mapa1_original = pygame.image.load("mapa.png").convert()
mapa2_original = pygame.image.load("mapa2.png").convert()

mapa1 = pygame.transform.scale(mapa1_original,(ANCHO,ALTO))
mapa2 = pygame.transform.scale(mapa2_original,(ANCHO,ALTO))
