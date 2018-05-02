Multigpu automation for WaltonChain miner: 1.7.0

If you want to change the directory asusmptions, they can be fairly easily modified at the top of the script.

Directory Struture Assumptions: 
You have a directory structure of:
C:\Walton-GPU-641
C:\Walton-GPU-642
C:\Walton-GPU-643 etc

Walton-GPU-641/                                                              
├── genesis.json                                                             
├── GPUMing_v0.2                                                             
│   ├── 0202001                                                              
│   ├── cudart32_80.dll                                                      
│   ├── cudart64_80.dll                                                      
│   ├── ming_run.iobj                                                        
│   ├── ming_run.ipdb                                                        
│   ├── ming_run.pdb                                                
├── pthreadVC2.dll                                                           
├── readme.txt                                                               
├── start_gpu.bat                                                                                                                                 
└── walton1.exe                                                                                

Walton.exe should also be renamed to walton 1, walton 2, etc.

Port Assumptions:
The script assumes that you have setup your multiGPU setup with ascending ports, from walton1 = 30303, 8545.  Walton2 = 30304,8546, etc.

Exiting and logging:
Press and hold scroll lock untill you see the tool tip change to "Scroll Lock Behind Held Down, Shutting Down", the script will log each miner and exit all processes including itself.
Another way to exit without logging is simply right clicking the .exe in the taskbar and selecting quit. 

MultiGPU: The default is setup for 1 GPU, a quick edit at the top to $NUM_GPUS set to another value, such as 2,3,4 etc will spawn these extra processes at the corresponding ports.

0.6 Goals: Better user interface.



