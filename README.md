# Nowcasting-PE-NAVs
This code demonstrates a PE fund-specific State Space Model developed in "Nowcasting Net Asset Value: The Case of Private Equity" by G.Brown, E.Ghysels, O.Gredil and publication in The Review of Financial Studie, Volume 36, Issue 3, March 2023, Pages 945–986: The Review of Financial Studies, Volume 36, Issue 3, March 2023, Pages 945–986.  
An earlier version is available on SSRN https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3507873.
The code reproduces the estimates for a hypothetical buyout fund that is plotted in Figure 1 of the paper. 

Instructions for the Matlab version:
1) Open FigureOne_MAINcode.m in Matlab 2018 or higher that has Econometrics toolbox. 
2) Make sure your Matlab directory references the directory with the content from the Github archive.
3) Select the options described in lines 3-to-17.
4) Run FigureOne_MAINcode.m

The fund data are hypothetical and simulated from the process described in Internet Appendix to the paper (Section A.6) at weekly frequency.
The fund operated for 562 weeks and had the true (arithmetic) alpha of 0 and the true market beta of 1.19. The reported NAVs were smoothed at lambda=0.9 and subject to a noise with a standard deviation of 5% (i.e. true sigma_n=0.05). 

The ``naive'' weekly NAV estimates (NAVweeklyEst) were constructed as described in Section A.3 of the Internet Appendix---https://www.dropbox.com/scl/fi/n0l2cf6flx6y7jtwehky5/OnlineAppendix__BGG_NowcastingPE4ssrn.pdf?rlkey=9ymjdlp3joxdzs3vec0l1tb65&dl=0 
The initial asset-to-return mapping is computed from these estimates using equation 4 of the main text with NAVweeklyEst in place of Vt. 

INDEMNIFICATION: The authors carry no liability for the use of this code and data for any applications.
