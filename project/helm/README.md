## Helm Chart 

Place the Helm Chart files in this directory.

To stage:
helm install techtrends helm/techtrends/ -f helm/techtrends/values-staging.yaml

To produce:
helm install techtrends helm/techtrends/ -f helm/techtrends/values-prod.yaml
