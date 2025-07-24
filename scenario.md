## Étape 1 : Créer un Pod Nginx

Nous allons commencer par créer un Pod contenant un conteneur Nginx.

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
