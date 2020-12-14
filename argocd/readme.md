for item in $(oc get Application,argocd,AppProject -o name); do oc get $item -o yaml > $(dirname $item)_$(basename $item).yaml ;done;
