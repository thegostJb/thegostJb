import pygame
import sys

# Initialisation de Pygame
pygame.init()

# Constantes
SCREEN_WIDTH = 800
SCREEN_HEIGHT = 600
FPS = 60

# Couleurs
WHITE = (255, 255, 255)
BLACK = (0, 0, 0)

# Création de la fenêtre du jeu
screen = pygame.display.set_mode((SCREEN_WIDTH, SCREEN_HEIGHT))
pygame.display.set_caption("Mon Jeu 2D")

# Boucle principale du jeu
clock = pygame.time.Clock()
running = True

while running:
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            running = False

    # Logique du jeu

    # Dessin
    screen.fill(BLACK)

    # Actualisation de l'affichage
    pygame.display.flip()

    # Limiter le nombre d'images par seconde
    clock.tick(FPS)

# Quitter Pygame
pygame.quit()
sys.exit()
