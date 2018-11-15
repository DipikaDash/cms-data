# cms-data 
#worked code for CMSSW_9_4_10_UCSBRice_v4 

1.scramv1 project -n CMSSW_9_4_10_UCSBRice_v4 CMSSW CMSSW_9_4_10
2.cd CMSSW_9_4_10_UCSBRice_v4/src/
3.cmsenv
4.git clone git@github.com:mkilpatr/13TeVAnalysis.git .
5.git checkout origin/94X
6.git submodule init
7.git submodule update
8.git clone git@github.com:mkilpatr/data.git
9.cd data/
10.unzip 13TeVAnalysis.zip
11.rm 13TeVAnalysis.zip
12.cd ..
13.scram b -j 10
