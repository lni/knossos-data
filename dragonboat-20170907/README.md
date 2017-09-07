edn files here are captured during Dragonboat's nightly tests. Over night, we started hundreds of thousands Raft clusters, we then randomly kill/restart nodes at very high churn rate. There are 64 background clients doing random writes/reads to generate background traffic. Another 32 clients are managed by the linearizability checker manager to performance and record their random write/read history. 

knossos tests didn't find any linearizability violation. 
