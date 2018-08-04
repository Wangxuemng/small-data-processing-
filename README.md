# small-data-processing-
Run routerless2.py and get total loops.
Then put the loops to rl8.txt 
Run test.py and put the result to rl8table.txt
Put rl8.txt and rl8table.txt to gem/config/topologies/
Run gem
./build/NULL/gem5.debug 
configs/example/garnet_synth_traffic.py  
--num-cpus=64  
--num-dirs=64  
--topology=RouterLess   
--mesh-rows=8  
--sim-cycles=100000  
--injectionrate=0.005  
--synthetic=Tornado
--network=garnet2.0

