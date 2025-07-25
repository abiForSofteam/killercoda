## Étape 1 : Créer un Pod Nginx

On commence par créer un Pod basé sur l’image `nginx`.

```yaml file=assets/pod.yaml
apiVersion: v1
kind: Pod
metadata:
  name: nginx
spec:
  containers:
  - name: nginx
    image: nginx
    ports:
    - containerPort: 80
