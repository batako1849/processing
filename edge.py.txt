import cv2
def capture_camera(mirror=True, size=None):
    cap = cv2.VideoCapture(0)



    while True:

        cap = cv2.GaussianBlur(cap,(3,3),0)
        lap = cv2.Laplacian(cap,cv2.CV_32F)
        edge_lap = cv2.convertScaleAbs(lap)

        cv2.imshow('img', edge_lap)



        k = cv2.waitKey(1) 
        if k == 27: 
            break

    cap.release()
    cv2.destroyAllWindows()