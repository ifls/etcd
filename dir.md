.
├── Documentation
│ └── dev-guide
│     └── apispec
│         └── swagger
├── api
│ ├── authpb
│ ├── etcdserverpb  rpc.proto是所有grpc服务的接口定义
│ │ └── gw
│ ├── membershippb
│ ├── mvccpb
│ ├── v3rpc
│ │ └── rpctypes
│ └── version
├── client go客户端sdk
│ ├── pkg
│ │ ├── fileutil
│ │ ├── logutil
│ │ ├── pathutil
│ │ ├── srv
│ │ ├── systemd
│ │ ├── testutil
│ │ ├── tlsutil
│ │ ├── transport
│ │ └── types
│ ├── v2
│ └── v3
│     ├── clientv3util
│     ├── concurrency
│     ├── credentials
│     ├── experimental
│     │ └── recipes
│     │     └── grpc_gateway
│     ├── internal
│     │ ├── endpoint
│     │ └── resolver
│     ├── leasing
│     ├── mirror
│     ├── mock
│     │ └── mockserver
│     ├── namespace
│     ├── naming
│     │ ├── endpoints
│     │ │ └── internal
│     │ └── resolver
│     ├── ordering
│     ├── snapshot
│     └── yaml
├── contrib  非核心代码
│ ├── lock
│ │ ├── client
│ │ └── storage
│ ├── mixin
│ ├── raftexample
│ └── systemd
│     ├── etcd3-multinode
│     └── sysusers.d
├── etcdctl
│ ├── ctlv2
│ │ └── command
│ ├── ctlv3
│ │ └── command
│ └── doc
├── etcdutl
│ ├── etcdutl
│ └── snapshot
├── hack
│ ├── benchmark
│ ├── insta-discovery
│ ├── kubernetes-deploy
│ ├── patch
│ └── tls-setup
│     └── config
├── pkg
│ ├── adt
│ │ └── img
│ ├── cobrautl
│ ├── contention
│ ├── cpuutil
│ ├── crc
│ ├── debugutil
│ ├── expect
│ ├── flags
│ ├── grpc_testing
│ ├── httputil
│ ├── idutil
│ ├── ioutil
│ ├── netutil
│ ├── osutil
│ ├── pbutil
│ ├── proxy
│ │ └── fixtures
│ ├── report
│ ├── runtime
│ ├── schedule
│ ├── stringutil
│ ├── traceutil
│ └── wait
├── raft
│ ├── confchange
│ │ └── testdata
│ ├── quorum
│ │ └── testdata
│ ├── raftpb
│ ├── rafttest
│ ├── testdata
│ └── tracker
├── scripts
├── server
│ ├── auth 访问权限
│ ├── config
│ ├── datadir
│ ├── embed
│ ├── etcdmain
│ ├── etcdserver
│ │ ├── api
│ │ │ ├── etcdhttp
│ │ │ ├── membership
│ │ │ ├── rafthttp
│ │ │ ├── snap
│ │ │ │ └── snappb
│ │ │ ├── v2auth
│ │ │ ├── v2discovery
│ │ │ ├── v2error
│ │ │ ├── v2http
│ │ │ │ ├── httptypes
│ │ │ │ └── testdata
│ │ │ ├── v2stats
│ │ │ ├── v2store
│ │ │ ├── v2v3
│ │ │ ├── v3alarm
│ │ │ ├── v3client
│ │ │ ├── v3compactor
│ │ │ ├── v3election
│ │ │ │ └── v3electionpb
│ │ │ │     └── gw
│ │ │ ├── v3lock
│ │ │ │ └── v3lockpb
│ │ │ │     └── gw
│ │ │ └── v3rpc
│ │ └── cindex
│ ├── lease 租约
│ │ ├── leasehttp
│ │ └── leasepb
│ ├── mock
│ │ ├── mockstorage
│ │ ├── mockstore
│ │ └── mockwait
│ ├── mvcc 多版本并发控制以及watch
│ │ ├── backend
│ │ │ └── testing
│ │ └── buckets
│ ├── proxy 网络协议转化
│ │ ├── grpcproxy
│ │ │ ├── adapter
│ │ │ └── cache
│ │ ├── httpproxy
│ │ └── tcpproxy
│ ├── verify
│ └── wal 日志
│     └── walpb
├── tests
│ ├── docker-dns
│ │ ├── certs
│ │ ├── certs-common-name-auth
│ │ ├── certs-common-name-multi
│ │ ├── certs-gateway
│ │ ├── certs-san-dns
│ │ ├── certs-wildcard
│ │ └── insecure
│ ├── docker-dns-srv
│ │ ├── certs
│ │ ├── certs-gateway
│ │ └── certs-wildcard
│ ├── docker-static-ip
│ │ ├── certs
│ │ └── certs-metrics-proxy
│ ├── e2e
│ ├── fixtures
│ ├── functional
│ │ ├── agent
│ │ ├── cmd
│ │ │ ├── etcd-agent
│ │ │ ├── etcd-proxy
│ │ │ ├── etcd-runner
│ │ │ └── etcd-tester
│ │ ├── rpcpb
│ │ ├── runner
│ │ ├── scripts
│ │ └── tester
│ └── integration
│     ├── client
│     │ └── examples
│     ├── clientv3
│     │ ├── concurrency
│     │ ├── connectivity
│     │ ├── examples
│     │ ├── experimental
│     │ │ └── recipes
│     │ ├── lease
│     │ ├── naming
│     │ └── snapshot
│     ├── embed
│     ├── fixtures-expired
│     ├── proxy
│     │ └── grpcproxy
│     ├── snapshot
│     │ └── testdata
│     └── v2store
└── tools
    ├── benchmark
    │ └── cmd
    ├── etcd-dump-db
    ├── etcd-dump-logs
    │ ├── expectedoutput
    │ └── testdecoder
    ├── etcd-dump-metrics
    ├── local-tester
    │ └── bridge
    └── mod

225 directories
