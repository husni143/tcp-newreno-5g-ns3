#TCP NewReno with varying 5G Bandwidth

This project investigates TCP NewReno performance under varying bandwidth using real 5G measurements from Bredbandskollen.

##Environment
- ns-3.48
- ubuntu linux
- TCP NewReno
- Two-node point-to.point network

##Running the simulation
copy tcp-5g.cc to the ns-3 scratch directory.

Run from the ns-3 root directory: 
     ./ns3 run scratch/tcp-5g

## Measurements

The link bandwidth changes at:

- 0 s: 49.96 Mbps
- 5 s: 145.23 Mbps
- 10 s: 184.67 Mbps
- 15 s: 256.59 Mbps
- 20 s: 156.95 Mbps

## Results

tcp-throughput.csv contains TCP throughput measurements.
tcp-cwnd.csv contains congestion window measurements.
newreno-fixed.png compares link bandwidth with TCP throughput.
newreno-cwnd-log.png displays congestion window over time.
