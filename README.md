# cms-data 
#worked code for CMSSW_9_4_10_UCSBRice_v4 

scramv1 project -n CMSSW_9_4_10_UCSBRice_v4 CMSSW CMSSW_9_4_10
cd CMSSW_9_4_10_UCSBRice_v4/src/
cmsenv
git clone git@github.com:mkilpatr/13TeVAnalysis.git .
git checkout origin/94X
git submodule init
git submodule update
git clone git@github.com:mkilpatr/data.git
cd data/
unzip 13TeVAnalysis.zip
rm 13TeVAnalysis.zip
cd ..
scram b -j 10
