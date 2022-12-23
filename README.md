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
root@test-pod-cx-pressure-client-04:/test# python3 /home/smallfile/smallfile_cli.py --operation read --top /test/small --threads 8 --files 2000 --file-size 15 --record-size 15 --fsync N
                                 version : 3.2
                           hosts in test : None
                        launch by daemon : False
                   top test directory(s) : ['/test/small']
                               operation : read
                            files/thread : 2000
                                 threads : 8
           record size (KB, 0 = maximum) : 15
                          file size (KB) : 15
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
                    finish all requests? : N
                              stonewall? : Y
                 measure response times? : N
                            verify read? : Y
                                verbose? : N
                          log to stderr? : N


host = test-pod-cx-pressure-client-04,thr = 00,elapsed = 1.6982908248901367,files = 2000,records = 2000,status = ok
host = test-pod-cx-pressure-client-04,thr = 01,elapsed = 1.7200579643249512,files = 1979,records = 1979,status = ok
host = test-pod-cx-pressure-client-04,thr = 02,elapsed = 1.7189781665802002,files = 1979,records = 1979,status = ok
host = test-pod-cx-pressure-client-04,thr = 03,elapsed = 1.751081943511963,files = 1979,records = 1979,status = ok
host = test-pod-cx-pressure-client-04,thr = 04,elapsed = 1.6938464641571045,files = 2000,records = 2000,status = ok
host = test-pod-cx-pressure-client-04,thr = 05,elapsed = 1.6990389823913574,files = 2000,records = 2000,status = ok
host = test-pod-cx-pressure-client-04,thr = 06,elapsed = 1.704685926437378,files = 2000,records = 2000,status = ok
host = test-pod-cx-pressure-client-04,thr = 07,elapsed = 1.7004704475402832,files = 1979,records = 1979,status = ok
total threads = 8
total files = 15916
total IOPS = 9304
total data =     0.228 GiB
 99.47% of requested files processed, warning threshold is  70.00%
elapsed time =     1.751
files/sec = 9304.533811
IOPS = 9304.533811
MiB/sec = 136.296882

```
