
https://github.com/ParamjeetSingh29/Video---Frame-Counter/assets/150776496/6f5805eb-be6b-43ef-b505-76989757daa7
# Video---Frame-Counter
import cv2

cap=cv2.VideoCapture("D:/Python Projects/frames/Video/WhatsApp Video 2023-12-23 at 11.37.10_1495097d.mp4")

i=0
while(cap.isOpened()):
    flag,frame=cap.read()
    if flag==False:
        break
    path='D:/Python Projects/frames/Frames/no of frames'+str(i)+'.jpg'
    cv2.imwrite(path,frame)
    i+=1

cap.release()
cv2.destroyAllWindows()
# Video
Uploading WhatsApp Video 2023-12-23 at 11.37.10_1495097d.mp4…
