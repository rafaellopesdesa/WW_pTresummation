Some information:


   1. norm[E,index] is the total cross section. E is the energy (7, 8, or 14 TeV). Index has the following convention:

         0 ... central value
         1 ... resummation scale up        (Qup)
         2 ... resummation scale down      (Qdown)
         3 ... renormalization scale up    (Rup)
         4 ... renormalization scale down  (Rdown)


      by definition, Qup and Qdown don't change the total cross section. Rup and Rdown do. So, if you want to estimate just the acceptance uncertainty, you have to normalize with values in norm[].

   2. total[E,index] has the WW pT differential distribution following the same convention as above.
   
         a) This has to be compared to the WW pT distribution *after* QCD showering (pythia or herwig). Otherwise you are not comparing apples to apples.
         b) The bins are 0.25 wide... this should be more than enough for us.

   3. The procedure is simple, generate events without any cut and make the same histogram. Calculate the ratio bin-by-bin. Use that to reweight your events. The Q and R variation should give your uncertainties.


Please! Please! Please! Cite the following paper: http://arxiv.org/abs/1407.4481
   
   
   
