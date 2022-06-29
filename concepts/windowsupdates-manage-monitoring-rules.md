---
title: 使用 Windows 更新 for Business 部署服务管理监视规则
description: 使用 Windows 更新 for Business 部署服务创建监视规则或恢复由监视规则暂停的部署。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 30f2c9cd2d219710fda5beba6862e9f15c7c94d6
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437448"
---
# <a name="manage-monitoring-rules-using-the-windows-update-for-business-deployment-service"></a>使用 Windows 更新 for Business 部署服务管理监视规则

对于部署服务发起的部署，可以使用监视规则根据部署信号配置警报和自动化操作。

监视规则与Windows 10功能更新的部署兼容。

## <a name="step-1-create-a-monitoring-rule"></a>步骤 1：创建监视规则

可以通过配置[监视设置](/graph/api/resources/windowsupdates-monitoringsettings)为部署创建[监视规则](/graph/api/resources/windowsupdates-monitoringrule)。 每个 [部署](/graph/api/resources/windowsupdates-deployments) 一次可以有一个活动监视规则。

监视规则由三个组件组成：
* **信号**：部署服务要监视的更新问题的类型。
* **阈值**：当此百分比的设备发出指定信号时，将触发监视规则。
* **操作**：触发监视规则时要执行的操作。

下面是创建部署的同时为部署创建监视规则的示例。

### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
        "version": "20H2"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "monitoring": {
            "monitoringRules": [
                {
                    "signal": "rollback",
                    "threshold": 5,
                    "action": "pauseDeployment"
                }
            ]
        }
    }
}
```

### <a name="response"></a>响应

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "id": "b5171742-1742-b517-4217-17b5421717b5",
    "state": {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
        "value": "offering",
        "reasons": [
            {
                "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason",
                "value": "offeringByRequest"
            }
        ],
        "requestedValue": "none",
        "effectiveSinceDate": "String (timestamp)"
    },
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
        "version": "20H2"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "monitoring": {
            "monitoringRules": [
                {
                    "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
                    "signal": "rollback",
                    "threshold": 5,
                    "action": "pauseDeployment"
                }
            ]
        },
        "rollout": null,
        "userExperience": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-2-resume-a-deployment-that-was-paused-by-a-monitoring-rule"></a>步骤 2：恢复由监视规则暂停的部署
当监视规则触发时，它提供了调查可能导致其应用的更新问题的机会。 调查后，你可能希望恢复部署。 有两种方法可以执行此操作：删除监视规则或更新监视规则阈值。

### <a name="example-resume-deployment-by-removing-a-monitoring-rule"></a>示例：通过删除监视规则来恢复部署
当触发暂停部署的监视规则时，恢复部署的一种方法是删除规则。

下面是通过删除规则来恢复部署的示例。

#### <a name="request"></a>请求

``` http
PATCH https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "monitoring": {
            "monitoringRules": []
        }
    }
}
```

#### <a name="response"></a>响应

``` http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "id": "b5171742-1742-b517-4217-17b5421717b5",
    "state": {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
        "value": "offering",
        "reasons": [
            {
                "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason",
                "value": "offeringByRequest"
            }
        ],
        "requestedValue": "none",
        "effectiveSinceDate": "String (timestamp)"
    },
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
        "version": "20H2"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "monitoring": {
            "monitoringRules": []
        },
        "rollout": null,
        "userExperience": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

### <a name="example-resume-deployment-by-updating-a-monitoring-rule-threshold"></a>示例：通过更新监视规则阈值来恢复部署
恢复部署的另一种方法是更改相关监视规则的阈值。 达到新阈值后，此操作 (， `pauseDeployment`) 会再次触发。 

下面是通过更改监视规则阈值来恢复部署的示例。 此示例还演示了如何编辑任何现有监视规则（即使其阈值尚未达到）以及如何在未达到此阈值的部署上创建监视规则。

#### <a name="request"></a>请求

``` http
PATCH https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "monitoring": {
            "monitoringRules": [
                {
                    "signal": "rollback",
                    "threshold": 10,
                    "action": "pauseDeployment"
                }
            ]
        }
    }
}
```

#### <a name="response"></a>响应

``` http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "id": "b5171742-1742-b517-4217-17b5421717b5",
    "state": {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
        "value": "offering",
        "reasons": [
            {
                "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason",
                "value": "offeringByRequest"
            }
        ],
        "requestedValue": "none",
        "effectiveSinceDate": "String (timestamp)"
    },
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
        "version": "20H2"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "monitoring": {
            "monitoringRules": [
                {
                    "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
                    "signal": "rollback",
                    "threshold": 10,
                    "action": "pauseDeployment"
                }
            ]
        },
        "rollout": null,
        "userExperience": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```
