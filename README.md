#!/usr/bin/env python3
# -*- coding: utf-8 -*-
"""
Created on Mon Jan 17 14:00:56 2022

@author: edwardlu
"""

import pygame

white = (225,225,225)

pygame.init()

size = (700,500)
screen = pygame.display.set_mode(size)
pygame.display.set_caption("滑鼠")

done= False
clock = pygame.time.Clock()

while not done:
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
           done = True
        if event.type == pygame.MOUSEBUTTONDOWN:
            pos =
            pygame.mouse.get_pos()
            print(pos)
            
screen.fill(white)
    pygame.draw.rect(screen, RED, [x + 10, y + 10, 10, 10])
    
    pygame.display.flip()

    clock.tick(60)

pygame.quit()
