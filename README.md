# SPEC SPRINTERS

### STEPS TO DOWNLOAD CHAMPSIM AND FILES

- Download ChampSim repository from [here](https://github.com/ChampSim/ChampSim).
- Download the following traces from these links [SPEC](https://dpc3.compas.cs.stonybrook.edu/champsim-traces/speccpu/), [Graph Analytics](https://utexas.app.box.com/s/2k54kp8zvrqdfaa8cdhfquvcxwh7yn85/folder/132804598561) and [SAT Solver](https://www.dropbox.com/sh/xs2t9y4cuqlgrlp/AACpzGOj6BcSB-BUolGaBjbta?dl=0).
  * `602.gcc_s-2226B.champsimtrace.xz`
  * `605.mcf_s-665B.champsimtrace.xz`
  * `605.mcf_s-782B.champsimtrace.xz`
  * `621.wrf_s-6673B.champsimtrace.xz`
  * `649. fotonik3d_s-10881B.champsimtrace.xz`
  * `654.roms_s-1007B.champsimtrace.xz.`
  * `654.roms_s-523B.champsimtrace.xz.`
  * `bfs-10.trace.gz(from Graph Analytics).`
  * `cadical-high-60K-1227B.champsimtrace.xz(from SAT Solver).`
- Place these files into `ChampSim/dpc3_traces` folder 
- Download the source code of Spec Sprinters
- Place `ipcp.l1d_pref`, `ipcp.l2c_pref`, `ipcp.llc_pref` files inside `ChampSim/prefetcher` folder

### STEPS TO RUN THE CODE
In ChampSim Folder run the following commands to get the output after IPCP prefetching.
  * `./build_champsim.sh bimodal no ipcp ipcp ipcp lru 1`
  * `./run_champsim.sh bimodal-no-ipcp-ipcp-ipcp-lru-1core 30 30 [TRACE NAME]`
  * `cat results_30M/[TRACE NAME]-bimodal-no-ipcp-ipcp-ipcp-lru-1core.txt`
- Now we can see results on terminal which contains parameters like IPC, mpkc, cache hits, cache misses and many more.


### Presentation
 Please refer to this [presentation](https://docs.google.com/presentation/d/1cNY_NGp6AePsVlPmW1K7c6n6JXECOSeP/edit?usp=sharing&ouid=117917141028873045506&rtpof=true&sd=true) and [video](https://youtu.be/SwNjS9jtsUM) for better understanding.

### References
- [IPCP paper](https://www.cse.iitk.ac.in/users/biswap/IPCP_ISCA20.pdf)

- [IPCP 1.0 presentation](https://dpc3.compas.cs.stonybrook.edu/slides/bouquet.pdf)
### Contributions

| Name                          	| Contribution 	|
|-------------------------------	|--------------	|
| G Lohith Reddy (210050054)       	|        Code changes, Presentation, Video     |
| G Adithya Rao (210050060)        	|        Code changes, Presentation, Video    |
| I Nithin (210050071)    	|        Code changes, Presentation, Video     	|
