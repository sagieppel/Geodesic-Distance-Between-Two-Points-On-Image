# Geodesic-Distance-Between-Two-Points-On-Image
Find minimal Geodesic distance between point two point (x0,y0 and x1,y1) on image (Im)

%Find minimal Geodesic distance between point two point (x0,y0 and x1,y1) on image (Im)
%The image can be color or grayscale
%return geodesic distance between x0,y0 and x1,y1

%Use the image as topological map with color as height and use the
%Dijkstra's algorithm to find minimal geodesic distance between x1,y1 and x0,y0

%Input:

%Im color image (or other multichannel image)

%x0,y0 coordinates (on the image) of the origin point
%x1,y1 Cordinates of the target point

%NumSteps optional parameter that allow  you to limit the number of cycle of the calculation this may result faster but less accurate calculation

%WeightDist the distance component have two parts distance travel on
%the image plane and distance in the color/grayscale value this parameter
%control the relative weight of the distance on the image plane

%Output:
%DistMap a map of geodesic distance to coordinate x0,y0

%Method:
%Use  the image as topological map and use the Dijkstra's algorithm to find geodesic distance
