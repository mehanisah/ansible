
$ helm install kubernetes-dashboard . --namespace kubernetes-dashboard -f values.yaml
$ helm upgrade kubernetes-dashboard . --namespace kubernetes-dashboard -f values.yaml
$ helm uninstall kubernetes-dashboard --namespace kubernetes-dashboard


$ kubectl create -f k8s-dashboard-account.yaml
serviceaccount/admin-user created
clusterrolebinding.rbac.authorization.k8s.io/admin-user created

$ kubectl -n kube-system create token admin-user
eyJhbGciOiJSUzI1NiIsImtpZCI6ImFaS1VCcDdPckNQWkhlNzl2bnNoelVZdGwxOUtUSmpjMThaUWNHQWdxNkEifQ.eyJhdWQiOlsiaHR0cHM6Ly9rdWJlcm5ldGVzLmRlZmF1bHQuc3ZjLmNsdXN0ZXIubG9jYWwiLCJrM3MiXSwiZXhwIjoxNzM4MzMwNTY4LCJpYXQiOjE3MzgzMjY5NjgsImlzcyI6Imh0dHBzOi8va3ViZXJuZXRlcy5kZWZhdWx0LnN2Yy5jbHVzdGVyLmxvY2FsIiwianRpIjoiYmU0ZmRlMWYtY2MwZC00Yjk5LWFmZjAtODM5NmU1MDFiYjhhIiwia3ViZXJuZXRlcy5pbyI6eyJuYW1lc3BhY2UiOiJrdWJlLXN5c3RlbSIsInNlcnZpY2VhY2NvdW50Ijp7Im5hbWUiOiJhZG1pbi11c2VyIiwidWlkIjoiMWMzZmViYzMtZjgwYy00MmVkLWExMjUtMGZkZWJiNjI4OTA5In19LCJuYmYiOjE3MzgzMjY5NjgsInN1YiI6InN5c3RlbTpzZXJ2aWNlYWNjb3VudDprdWJlLXN5c3RlbTphZG1pbi11c2VyIn0.oG1NDs4_5z5wzwu-6wLrHnP7ieoIMf591uzeK0J5ttu0AmmGSnX9M-gzgb6HVXIKo9NIj3zSkibslMgvlArSa3sjoFq8U4dGVvUp8fvZGXhhPTQzDV681Ww57mJXhljPrF_yPHlxBP5k-vwA7UPD5nhnp01Q4Z3iEkZA5RdHfGwH0tA5amVO0Zhv_IevVk-zRarV_78m53bKCA2XYWTrDotTXDFgVgXfURh10X7wJ45-5-CN3ktGtWEeuaotpkDWqQnf-77CQS6kjoC5X8VhxIPL7j2OuFcqO-My_Tt-VTvVsAQuwAAuEnsoawY8f1G76kqrzoHgm3hE4fJTGpEqOQ
