```sh

root@test-pod-cx-pressure-client-04:/test# python3 /home/smallfile/smallfile_cli.py --top /test/small --threads 8 --files 2000 --file-size 15 --record-size 15 --fsync N --operation create
changing --finish to true for op type create
                                 version : 3.2
                           hosts in test : None
                        launch by daemon : False
                   top test directory(s) : ['/test/small']
                               operation : create
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
                    finish all requests? : Y
                              stonewall? : Y
                 measure response times? : N
                            verify read? : Y
                                verbose? : N
                          log to stderr? : N
host = test-pod-cx-pressure-client-04,thr = 00,elapsed = 5.390785455703735,files = 1979,records = 1979,status = ok
host = test-pod-cx-pressure-client-04,thr = 01,elapsed = 5.397075891494751,files = 2000,records = 2000,status = ok
host = test-pod-cx-pressure-client-04,thr = 02,elapsed = 5.347317457199097,files = 2000,records = 2000,status = ok
host = test-pod-cx-pressure-client-04,thr = 03,elapsed = 5.380971431732178,files = 2000,records = 2000,status = ok
host = test-pod-cx-pressure-client-04,thr = 04,elapsed = 5.386497974395752,files = 1979,records = 1979,status = ok
host = test-pod-cx-pressure-client-04,thr = 05,elapsed = 5.398409605026245,files = 1979,records = 1979,status = ok
host = test-pod-cx-pressure-client-04,thr = 06,elapsed = 5.389926195144653,files = 2000,records = 2000,status = ok
host = test-pod-cx-pressure-client-04,thr = 07,elapsed = 5.408523797988892,files = 1979,records = 1979,status = ok
total threads = 8
total files = 15916
total IOPS = 2954
total data =     0.228 GiB
 99.47% of requested files processed, warning threshold is  70.00%
elapsed time =     5.409
files/sec = 2954.334433
IOPS = 2954.334433
MiB/sec = 43.276383

```
