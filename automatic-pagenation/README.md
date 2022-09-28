`spang2` can obtain results from *Virtuoso* by **automatic pagenation**.

Example SPARQL query:
```
# @endpoint https://www.orpha.net/sparql

PREFIX oboInOwl: <http://www.geneontology.org/formats/oboInOwl#>

SELECT ?s ?o
WHERE {
    ?s oboInOwl:hasDbXref ?o
}
```

Obtain data from SPARQL endpoint.
```
$ spang2 orphanet.rq > orphanet.tsv
Querying for the next page (OFFSET 10000 LIMIT 10000)...
Querying for the next page (OFFSET 20000 LIMIT 10000)...
Querying for the next page (OFFSET 30000 LIMIT 10000)...
Querying for the next page (OFFSET 40000 LIMIT 10000)...
$ wc orphanet.tsv
  42571   85142 3791019 orphanet.tsv
```

You can also execute the query file as follows, if the
file includes shebang line.
```
$ orphanet.rq > orphanet.tsv
```

Even without the query file, you can execute spang comand-line shortcuts equivalent to the query file.
```
$ spang2 -e orphanet -P oboInOwl:hasDbXref > orphanet.tsv
```

Extract subset of tsv to make Turtle.
```
$ ./orphanet-ensembl.sh > orphanet-ensembl.ttl
$ grep -c ensembl orphanet-ensembl.ttl
3213
```

You can also use FILTER at the SPARQL level to extract the subset (see
`orphanet_filter.rq`).
