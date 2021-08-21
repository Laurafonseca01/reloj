horizontal_position= 0
horizontal_positionm= 0
horizontal_positionh= 0

def setup():
    size(400, 400)
    
def draw():
    global horizontal_position
    background(191)
    
    fill (200)
    square(horizontal_position, 157, 45)
    
    if horizontal_position > height:
        horizontal_position = 0
    
    else:
          horizontal_position = map(second(), 0, 59, 0, height)
          
    global horizontal_positionm
          
    fill (130)
    square(horizontal_positionm, 204, 50)
    
    if horizontal_positionm > height:
        horizontal_positionm = 0
        
    else:
        horizontal_positionm = map(minute(), 0, 59, 0, height)
        
    global horizontal_positionh
    
    fill (0)
    square(horizontal_positionh, 258, 75)
    
    if horizontal_positionh > height:
        horizontal_positionh = 0
        
    else:
        horizontal_positionh = map(hour(), 0, 23, 0, height)




        