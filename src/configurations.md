# Configurations

## Configuration A
  Most efficient config and has miner-selected txs, what everyone should aim to implement
  long-term.

![Configuration A](img/configurations/a-sv2-group-channel-miner-tx.png)

## Configuration B
  Most efficient config and has pool-selected txs.

![Configuration B](img/configurations/b-sv2-group-channel-HOM-pool-tx.png)

## Configuration C
  MVP1

![Configuration C](img/configurations/c-sv1-sv2-translator-proxy-pool-tx.png)

## Configuration D
  TODO: MVP2

<!-- ![Configuration D]() -->

```
SV1 MD <- sv1 conn -> SV1/SV2 Translator Proxy <- ext chnl -> SV2 Pool <-> TP
                              |
                              TP
```

## Configuration E
  More efficient than SV1, but one of the least efficient configs. Important because currently the only SV2 production pool (Braiins), supports Standard Channels.

![Configuration E](img/configurations/e-sv2-std-chnl-no-proxy.png)

## Configuration F
  Not recommended because if a miner is running a proxy, they should always favor group channels, but
  shown for the sake of completeness.

![Configuration F](img/configurations/f-sv2-std-chnl-proxy.png)

## Configuration G
   Atypical configuration, but shown to highlight protocol flexibility.
<!-- ![Configuration G]() -->

```
SV2 MD <- std chnl -> SV2 Proxy <- grp chnl -> SV2 Proxy <- grp chnl -> SV2 Pool <-> TP
```

## Configuration H
   Atypical configuration, but shown to highlight protocol flexibility.
<!-- ![Configuration H]() -->

```
SV2 MD <- std chnl -> SV2 Proxy <- grp chnl -> SV2 Proxy <- grp chnl -> SV2 Pool <-> TP
                         |
                         TP
```

# Stratum V1 Configurations

## Stratum V1 No Proxy
![Stratum V1 No Proxy](img/configurations/sv1-no-proxy.png)

## Stratum V1 Non-Standard Proxy
![Stratum V1 No Proxy](img/configurations/sv1-proxy.png)
