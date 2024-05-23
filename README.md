# Provider and Client Applications with Kubernetes

Bu proje, Minikube kullanarak yerel bir Kubernetes kümesi oluşturmayı ve yönetmeyi öğrenmek için tasarlanmıştır.
Provider ve client uygulamaları, Docker kapsayıcıları olarak Kubernetes kümesine dağıtılmıştır.
Kümenin durumunu ve podların ayrıntılarını görmek için Lens adlı bir Kubernetes yönetim aracı kullanılmıştır.

Gereklilikler:

Minikube kurulu
Kubectl kurulu

Kullanım:

minikube start komutunu kullanarak bir Minikube kümesi başlatın.
kubectl get nodes komutunu kullanarak kümenizin düğümlerini kontrol edin.
kubectl run komutunu kullanarak bir Docker kapsayıcısı dağıtın.
kubectl get pods komutunu kullanarak kümenizin pod'larını kontrol edin.
kubectl logs komutunu kullanarak bir pod'un günlüklerini görüntüleyin.
kubectl exec komutunu kullanarak bir pod'a bir komut çalıştırın.
kubectl delete pod komutunu kullanarak bir pod'u silin.
minikube stop komutunu kullanarak Minikube kümenizi durdurun.

Provider uygulamasını dağıtma:

kubectl apply -f provider-deployment.yaml
kubectl apply -f provider-service.yaml

Client uygulamasını dağıtma:

kubectl apply -f client-deployment.yaml
kubectl apply -f client-service.yaml

Podları Lens üzerinden görüntüleme:

Lens'i açın ve Kubernetes kümenize bağlanın.
"Podlar" sekmesine gidin.
Provider ve client uygulamalarına ait podları arayın.
Bir pod'a tıklayarak ayrıntılarını görüntüleyin.

Sorun Giderme:

Minikube'u başlatırken sorun yaşıyorsanız, bilgisayarınızda yeterli RAM ve CPU olduğundan emin olun.
Kubectl'i kullanırken sorun yaşıyorsanız, Minikube kümenizin çalıştığından ve kubectl'in kümenize doğru şekilde yapılandırıldığından emin olun.
