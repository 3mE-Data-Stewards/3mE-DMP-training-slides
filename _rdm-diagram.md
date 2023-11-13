```{dot}
digraph G {

    subgraph cluster_0 {
        color=darkgrey;
        style=filled;
        fillcolor=lightgrey
        node [label="test"] D;
        node [label="test2"] B;
        node [label="test3"] C;

        label = "Analysis"

    }

  A [label="Conceptualisation"]
  B [label="Documentation" shape=note]
  C [label="Data Storage" shape=cylinder]
  D [label="Version control"]
  E [label="Backups" shape=box]
  F [label="Publication"]
  G [label="Security"]
  H [label="DMP"]
  
  A -> H -> {C,D,B} -> F
  C -> E
  C -> G

}
```
