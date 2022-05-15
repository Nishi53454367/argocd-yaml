# argocd-yaml
ArgoCDで使えるyamlのストック

# ファイル一覧
| フォルダ  |  ファイル  |  説明  |
| ---- | ---- | ---- |
|  argorollout  |  deployment.yaml  |  ブルー/グリーンデプロイ用deployment  |
|  argorollout  |  rollout-bluegreen-active-service.yaml  |  ブルー用service  |
|  argorollout  |  rollout-bluegreen-preview-service.yaml  |  グリーン用service  |
|  authority  |  CreateUser_ConfigMap.yaml  |  ユーザーを作成  |
|  authority  |  GrantRole_ConfigMap.yaml  |  作成したユーザーに権限を付与  |
|  authority  |  ProjectPolicy_AppProject.yaml  |  プロジェクトの権限を定義  |
|  google-managed-tls  |  argo-backend-config.yaml  | (GKE専用)GoogleマネージドSSL証明書の設定<br>https://argo-cd.readthedocs.io/en/stable/operator-manual/ingress/#creating-a-backendconfig |
|  google-managed-tls  |  argo-frontend-config.yaml  | (GKE専用)GoogleマネージドSSL証明書の設定<br>https://argo-cd.readthedocs.io/en/stable/operator-manual/ingress/#creating-a-frontendconfig |
|  google-managed-tls  |  ingress.yaml  | (GKE専用)GoogleマネージドSSL証明書の設定<br><br>以下を組み合わせて作成。<br>https://argo-cd.readthedocs.io/en/stable/operator-manual/ingress/#creating-an-ingress<br><br>https://cloud.google.com/kubernetes-engine/docs/how-to/managed-certs#setting_up_a_google-managed_certificate |
|  google-managed-tls  |  ManagedCertificate.yaml  | (GKE専用)GoogleマネージドSSL証明書の設定<br><br>以下をベースに`namespace: argocd`を指定。<br>https://cloud.google.com/kubernetes-engine/docs/how-to/managed-certs#setting_up_a_google-managed_certificate |
|  google-managed-tls  |  Service.yaml  | (GKE専用)GoogleマネージドSSL証明書の設定<br>https://argo-cd.readthedocs.io/en/stable/operator-manual/ingress/#creating-a-service |