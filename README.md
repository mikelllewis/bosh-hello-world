# Upload cloud config
```
cd ~/
git clone https://github.com/dazjones/bosh-cloud-configs
bosh ucc bosh-cloud-configs/gcp/cloud-config-europe-west-1.yml
```

# Create, upload and deploy release
```
cd ~/
git clone https://github.com/anthonysroberts/bosh-hello-world-compile
cd bosh-hello-world
bosh create-release
bosh upload-release
bosh -d bosh-hello-world-compile deploy manifest.yml
```
