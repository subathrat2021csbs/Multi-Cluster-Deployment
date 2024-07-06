Argo CD Setup

1.Install Argo CD
Command : 
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

2.Run Argo CD in HTTP Mode(Insecure)

3.Expose Argo CD Server Service in NodePort Mode
Command:
kubectl edit svc argocd-server -n argocd

4.Change the type to NodePort from ClusterIP

