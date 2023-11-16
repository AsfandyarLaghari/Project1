import pygame

pygame.init()

SCREEN_WIDTH = 800
SCREEN_HEIGHT = 600

screen = pygame.display.set_mode((SCREEN_WIDTH, SCREEN_HEIGHT))

run = True
while run:

    for event in pygame.event.get():
        if event.type == pygame.QUIT:
         run = False

    if event.type == pygame.MOUSEMOTION:
        print('Mouse is moving')

    if event.type == pygame.MOUSEWHEEL:
        print('Mouse is wheeling lol')

pygame.quit()

