from pygame import mixer
import datetime
from time import time
def loopformusic(music, stopper):
    mixer.init()
    mixer.music.load(music)
    mixer.music.play()
    while True:
        user_input = input()
        if user_input == stopper:
            mixer.music.stop()
            break

def forlog(my_input):
    with open("mylog.txt", "a") as f:
        f.write(f"{my_input} time : {datetime.datetime.now()}")

outer_water_time = time()
outer_eyes_time = time()
outer_exercise_time = time()
watertimer = 25*60
eyetimer = 30*60
exercisetimer = 45*60

while True:
    if time() - outer_water_time > watertimer:
        print("its reminder for water Enter 'drank' to stop")
        loopformusic("waterprog.mp3", "drank")
        outer_water_time = time()
        forlog("Drank water")

    if time() - outer_eyes_time > eyetimer:
        print("its a reminder for your eyes Enter 'eydone' to stop")
        loopformusic("eyes.mp3", "eydone")
        outer_eyes_time = time()
        forlog("eyes done ")

    if time() - outer_exercise_time > exercisetimer:
        print("its a reminder for exercise Enter 'exdone' to stop")
        loopformusic("exercisesong.mp3", "exdone")
        outer_exercise_time = time()
        forlog("exercise done ")

