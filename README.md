# aws-ready-sample-gitops

Sample GitOps content for the AWS-ready bootstrap from cloudnative-team/liferay-portal.

Mirrors the layout of [gcp-ready-sample-gitops](https://github.com/cloudnative-team/gcp-ready-sample-gitops).

Used to validate LCD-51065 (structured JSON logging) on AWS. `structuredLogging.enabled: true` is set in the base liferay.yaml so the inject script runs.

## Layout

```
liferay/
    system/
        infrastructure-provider.yaml
    projects/
        lcd-51065/
            base/
                infrastructure.yaml
                liferay.yaml
            environments/
                prd/
                    infrastructure.yaml
                    liferay.yaml
```
