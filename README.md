# gke-ftp-on-nfs-volume

Deploy a FTP server with Google Kubernetes Engine (GKE) using mounted nfs volumes backed by Google Compute Engine persistent disks.

## Requirements

Follow these instructions to deploy the NFS server
<https://github.com/reisbel/gke-nfs-persistence-volume>

## Steps

Clone repository

```bash
git clone https://github.com/reisbel/gke-ftp-on-nfs-volume.git && cd gke-ftp-on-nfs-volume
```

Create FTP deployment

```bash
kubectl apply -f config/ftp-deployment.yaml
```

Create FTP service

```bash
kubectl apply -f config/ftp-service.yaml
```

## References

<https://medium.com/platformer-blog/nfs-persistent-volumes-with-kubernetes-a-case-study-ce1ed6e2c266>

## License

MIT - See [LICENSE](LICENSE) for more information.
