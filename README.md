```sh

root@test-pod-cx-pressure-client-04:/test# python3 /home/smallfile/smallfile_cli.py --top /test/small --threads 1 --files 100000 --file-size 1 --operation cleanup
do not need pause between files for single-threaded workload
changing --finish to true for op type cleanup
                                 version : 3.2
                           hosts in test : None
                        launch by daemon : False
                   top test directory(s) : ['/test/small']
                               operation : cleanup
                            files/thread : 100000
                                 threads : 1
           record size (KB, 0 = maximum) : 0
                          file size (KB) : 1
                  file size distribution : fixed
                           files per dir : 100
                            dirs per dir : 10
              threads share directories? : N
                         filename prefix :
                         filename suffix :
             hash file number into dir.? : N
                     fsync after modify? : N
                         incompressible? : N
          pause between files (microsec) : 0
                             auto-pause? : N
 delay after cleanup per file (microsec) : 0
             minimum directories per sec : 50
                             total hosts : 1
                    finish all requests? : Y
                              stonewall? : Y
                 measure response times? : N
                            verify read? : Y
                                verbose? : N
                          log to stderr? : N
host = test-pod-cx-pressure-client-04,thr = 00,elapsed = 162.158433675766,files = 100000,records = 0,status = ok
total threads = 1
total files = 100000
100.00% of requested files processed, warning threshold is  70.00%
elapsed time =   162.158
files/sec = 616.68084
```
