# OCV-face68-2DOF-Rotation
OpenCV Face68 2DOF Rotation

## Kopf Winkel "ATAN"
```
Point centerPoint = new Point(points[pointUnten].x, points[pointUnten].y);
Point winkelPoint = new Point(points[pointOben].x, points[pointOben].y);
Imgproc.line(rgbMat, centerPoint, winkelPoint, new Scalar(255, 128, 128), 2);
double faceAngle = Math.Atan2(winkelPoint.y - centerPoint.y, winkelPoint.x - centerPoint.x) * 180.0f / Math.PI + 90.0f;
DMT.StaticStore.FaceAngle = faceAngle;
```
