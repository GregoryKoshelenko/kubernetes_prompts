# kubernetes_prompts
AI Prompts for kubernetes template generation

| NAME | PROMPT | DESCRIPTION | EXAMPLE |
|------|--------|-------------|---------|
| app-configmap | Generate a Pod manifest that uses a ConfigMap for environment variables and mounts. Specify: pod name, image, configMap name/key, env var, mount path. | Pod with env and volume from ConfigMap. | [yaml/app-configmap.yaml](yaml/app-configmap.yaml) |
| app-cronjob | Generate a CronJob manifest. Specify: name, schedule, image, command, restart policy. | CronJob running a command on schedule. | [yaml/app-cronjob.yaml](yaml/app-cronjob.yaml) |
| app-job-rsync | Generate a Job manifest to sync data from GCS using gsutil rsync. Specify: name, image, command, disk name, mount path, backoffLimit. | Job syncing GCS bucket to disk. | [yaml/app-job-rsync.yaml](yaml/app-job-rsync.yaml) |
| app-livenessprob | Generate a Pod manifest with HTTP liveness probe. Specify: pod name, namespace, image, container name, probe path/port, timings, containerPort. | Pod with HTTP liveness probe. | [yaml/app-livenessprob.yaml](yaml/app-livenessprob.yaml) |
| app-multi-containers | Generate a Pod manifest with two containers sharing an emptyDir volume. Specify: pod name, container names/images, volume name, mount paths, commands. | Two containers sharing a volume. | [yaml/app-multi-containers.yaml](yaml/app-multi-containers.yaml) |
| app-readinessprob | Generate a Pod manifest with HTTP liveness and readiness probes. Specify: pod name, image, container name, probe paths/ports, timings, containerPort. | Pod with liveness and readiness probes. | [yaml/app-readinessprob.yaml](yaml/app-readinessprob.yaml) |
| app-resource | Generate a Pod manifest with resource requests/limits and HTTP probes. Specify: pod name, image, container name, probe paths/ports, timings, resources, containerPort. | Pod with probes and resource limits. | [yaml/app-resource.yaml](yaml/app-resource.yaml) |
| app-secret-env | Generate a Pod manifest with env vars from a Secret. Specify: pod name, container name, image, secret name/keys, env var names, restart policy. | Pod with secret-based env vars. | [yaml/app-secret-env.yaml](yaml/app-secret-env.yaml) |
| app-secret-volume | Generate a Pod manifest that mounts a Secret as a volume. Specify: pod name, container name, image, secret name, volume name, mount path, readOnly. | Pod with secret mounted as volume. | [yaml/app-secret-volume.yaml](yaml/app-secret-volume.yaml) |
| app-labels | Generate a Pod manifest with custom labels. Specify: pod name, image, container name, labels, containerPort, port name. | Pod with custom labels. | [yaml/app-labels.yaml](yaml/app-labels.yaml) |
