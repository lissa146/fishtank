# fishtank
import pygame

pygame.init()  
pygame.display.set_caption("fishtank")  # sets the window title
screen = pygame.display.set_mode((1000, 1000))  # creates game screen
mousePos = (400,400)

castleImg = pygame.image.load("castle.png").convert_alpha()
while True:
    event = pygame.event.wait()
    if event.type == pygame.MOUSEMOTION:
        mousePos = event.pos
    print(mousePos)

    screen.fill((0,0,0))
    



    pygame.display.flip()#this actually puts the pixel on the screen
