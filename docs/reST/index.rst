import pygame
import sys

pygame.init()
wd_size = (700,400)

white = (255,255,255)
red = (255,0,0)

screen = pygame.display.set_mode(wd_size)
pygame.display.set_caption("Pygame Drawing Example")

img = pygame.image.load("image.jpg")

running = True

while running:
  for event in pygame.event.get():
    if event.type == pygame.QUIT:
      running = False

  screen.fill(white)
  screen.blit(img,(0,0))
  pygame.display.flip()

pygame.quit
sys.exit()
