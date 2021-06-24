# !pip install pygame
import pygame
import sys

# 1.Pygame 초기화
pygame.init()

# set caption
pygame.display.set_caption('Jumping dino')

# set screen
MAX_WIDTH = 800
MAX_HEIGHT = 400
screen = pygame.display.set_mode((MAX_WIDTH, MAX_HEIGHT))

# set FPS
fps = pygame.time.Clock()

# get image
imgDino1 = pygame.image.load('images/dino1.png')
imgDino2 = pygame.image.load('images/dino2.png')
# imgDinoWalk = [imgDino1, imgDino2]
dino_height = imgDino1.get_size()[1]
dino_bottom = MAX_HEIGHT - dino_height
dino_x = 50
dino_y = dino_bottom
jump_top = 200
wall = pygame.image.load('images/wall.PNG')
wall_height = wall.get_size()[1]
wall_bottom = MAX_HEIGHT - wall_height
wall_x = 650
wall_y = wall_bottom


is_bottom = True
is_go_up = False
left_leg = True

while True:
    # 흰 색 화면으로 설정하기
    screen.fill((255, 255, 255))
    
    # event check
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            pygame.quit()
            sys.exit()
        elif event.type == pygame.KEYDOWN:
            if is_bottom:
                is_go_up = True
                is_bottom = False

    # dino move
    if is_go_up:
        dino_y -= 10.0
        if dino_y <= jump_top: is_go_up = False
    
    else:
        if not is_bottom: 
            dino_y += 10.0
            
            if dino_y >= dino_bottom:
                is_bottom = True
                dino_y = dino_bottom
    
    if is_bottom:
        if left_leg: screen.blit(imgDino1, (dino_x, dino_y))
        else: screen.blit(imgDino2, (dino_x, dino_y))
        left_leg = not left_leg
    else: screen.blit(imgDino1, (dino_x, dino_y))
        
    wall_x -= 10
    if wall_x < 0:
        wall_x = 800
        
    # update
    screen.blit(wall, (wall_x, wall_y))
    pygame.display.update()
    fps.tick(30)
