# EOF

send data to `cat` command
```bash
cat << EOF
Hello World!
EOF
```

```yaml
kubectl apply -f << EOF
apiVersion: v1
kind: Pod
metadata:
  labels:
    run: nginx
  name: nginx
spec:
  containers:
  - image: nginx:apline
    name: nginx
EOF
```

save date to a `file` and send to `cat` command
```bash
cat << EOF > file
Hello World!
EOF
```

use other commands by getting data from terminal
```bash
wc -l << EOF
This is a simple lookup program 
for good (and bad) restaurants
in Cape Town.
EOF
```
