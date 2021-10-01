# TL;DR
```bash
helm repo add imgproxy https://helm.imgproxy.net/
helm upgrade -i imgproxy -f values.yml imgproxy/imgproxy
```
# Customize
- Check information in https://github.com/imgproxy/imgproxy-helm/tree/master/imgproxy
- Add custom env variables for the latest version of imgproxy:
  - Create `values.secret.yml` for secret key
  - ```
    helm upgrade -i imgproxy -f values.secret.yml imgproxy/imgproxy
    ```

# Change log
- Enable image fetching from Google Cloud Storage buckets https://docs.imgproxy.net/serving_files_from_google_cloud_storage