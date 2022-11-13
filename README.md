# kube.promtail
# kube.grafana

echo "# kube.grafana" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:thlasta/kube.promtail.git
git push -u origin main


# Repo clonen
git clone git@github.com:thlasta/kube.promtail.git

# Repo auschecken/holen
git pull git@github.com:thlasta/kube.promtail.git

# Bei Änderungen:
git commit -m "Änderungsbeschreibung"
git push --all

# Jump one folder up, and apply to the whole folder:
kubectl apply -f promtail/

# Namespace "monitoring" anlegen
kubectl create namespace monitoring