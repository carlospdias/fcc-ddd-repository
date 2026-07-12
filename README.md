# fcc-ddd-repository










curl -G -s \
  -H "User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64)" \
  --data-urlencode "q=g:org.hibernate.orm AND a:hibernate-core" \
  --data-urlencode "core=gav" \
  --data-urlencode "rows=5" \
  --data-urlencode "wt=json" \
  "https://central.sonatype.com/solrsearch/select" | jq '.response.docs[] | {versao: .v}'
