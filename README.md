```plaintext
ATLAS> 
EXTRACT> init inf="projeto3f1.log"
EXTRACT> extract name="nvt" (xintercept(maxslope(curve(abs(v."gate"),abs(i."drain")))) 	- abs(ave(v."drain"))/2.0)
nvt=0.803833837 
EXTRACT> extract name="nbeta" slope(maxslope(curve(abs(v."gate"),abs(i."drain")))) 	* (1.0/abs(ave(v."drain")))
nbeta=1.86624622e-05 
EXTRACT> extract name="ntheta" ((max(abs(v."drain")) * 1.86624622e-05)/max(abs(i."drain"))) - (1.0 / (max(abs(v."gate")) - (0.803833837)))
ntheta=0.028385805 
EXTRACT> 
EXTRACT> quit
quit
