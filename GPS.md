#####CONVERSIONS:
Earth Raduis=	6371000	M
RAD-DEG=	57.29564553	
DEG-RAD =	0.017453333			
E/N =	Positive				
W/S =	Negative

#####GIVEN TWO POINTS:
	      |LATT (φ)					                            |LON (λ)
POINT		|Degrees	Minute	Seconds	POLE	   RAD	      |Degrees	Minute	Seconds	POLE	    RAD
P1	    |   50	    3	      59	   N	 0.873825374	  |  5	      42	    53	    W	  -0.099740952
P2	    |   58	    38	    38	   N	 1.023531341	  |  3	      4	      12	    W	  -0.053581733


#####CALCULATIONS AND FORMULA:

DISTANCE BETWEEN TWO COORDINANTES										
a = sin²(Δφ/2) + cos φ1 ⋅ cos φ2 ⋅ sin²(Δλ/2)										
c = 2 ⋅ atan2( √a, √(1−a))   or  C = 2 ⋅ atan( √a/√(1−a))										
d = R ⋅ c										
"where φ is latitude, λ is longitude, R is earth’s radius (mean radius = 6,371km);
 note that angles need to be in radians to pass to trig functions! "										
										
Δφ =	0.149705967	RADIAN	Change in Lattitude between P1 and P2, Hence Δφ = (P2-P1) * DEGtoRAD							
Δλ =	0.046159219	RADIAN	Change in Longitude between P1 and P2, Hence Δφ = (P2-P1) * DEGtoRAD							
										
	sin²(Δφ/2)	cos φ1	cos φ2	sin²(Δλ/2)	RESULT		a	1-a		
a = 	0.005592513	0.641897992	0.52035361	0.000532574	0.0057704		0.0057704	0.9942296		
										
c =	0.152072786		C = 2 ⋅ atan( √(1−a)/√a)							
										
d =	968.8557173	km								
										
										
INITIAL BEARING @ P1										
 θ = atan2( sin Δλ ⋅ cos φ2 , cos φ1 ⋅ sin φ2 − sin φ1 ⋅ cos φ2 ⋅ cos Δλ ) 										
 θ = atan( sin(λ2-λ1) * cos(φ2)/ cos(φ1)*sin(φ2) - sin(φ1)*cos(φ2)*cos(λ2-λ1) ) 										
										
 Y=	sin(λ2-λ1) * cos(φ2);									
 Y=	0.024010587									
X=	"cos(φ1)*sin(φ2) - sin(φ1)*cos(φ2)*cos(λ2-λ1);
"									
X=	0.14957239									
 θ = 	ATAN(Y/X)									
 θ = 	9.119761697	DEG								
										
http://www.geomidpoint.com/destination/										
http://www.movable-type.co.uk/scripts/latlong.html										

