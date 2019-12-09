# Face_Detection_using_opencv
This code use opencv to recognize face in a given picture

- So are First step was we searched opencv on github
- Then we donwloaded the opencv project from github it included all algorithm for classification of face we are using haarcascade_frontalface_alt.xml
- I have uploaded the xml file of that algorithm in the project check the doc and xml file above
- okay so once you download the the xml file and project or you zip file of my project you can provide the path of that xml file which you just downloaded into your project
- This is the static implementation where model recognize the number of faces in the given picture 
- I have created a function called which will perform this operation
- def detect_faces_show(fpath):
  -    img = cv2.imread(fpath)
  -    gray = cv2.cvtColor(img,cv2.COLOR_BGR2RGB)
  -    faces = faceCascade.detectMultiScale(gray,scaleFactor=1.2,minNeighbors=2,minSize=(30,30),flags=cv2.CASCADE_SCALE_IMAGE)
  -    print("Found %d faces !"%len(faces))
    
  -    for(x,y,w,h)in faces:
  -        cv2.rectangle(img,(x,y),(x+w,y+h),(0,255,0),3)
  -        plt.imshow(cv2.cvtColor(img,cv2.COLOR_BGR2RGB))
  # OUTPUT
  
 
 
