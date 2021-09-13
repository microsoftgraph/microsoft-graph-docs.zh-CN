---
title: 使用 Windows Update for Business 部署服务管理部署的监视规则
description: 对于部署服务启动的部署，可以使用监视规则根据部署信号配置警报和自动操作。
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 1e4f0538a9e7a5d47b070514685a11860a86ac35
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117527"
---
# <a name="manage-monitoring-rules-for-a-feature-update-deployment-using-the-windows-update-for-business-deployment-service"></a>使用 Windows Update for Business 部署服务管理功能更新部署的监视规则

对于部署服务启动的部署，可以使用监视规则根据部署信号配置警报和自动操作。

监视规则与部署功能Windows 10兼容。

> [!NOTE]
> 如果在创建[部署时未指定](/graph/api/resources/windowsupdates-monitoringrule)监视规则，将创建默认[](/graph/api/resources/windowsupdates-deployment)监视规则。 此默认监视规则具有 **信号**、阈值 和 `rollback`  `20` **操作** `alertError` 。 在 API 的未来更新中，此行为将更改，并且不会创建默认监视规则。

## <a name="step-1-create-a-monitoring-rule"></a>步骤 1：创建监视规则

您可以通过配置 [监视](/graph/api/resources/windowsupdates-monitoringrule) 设置为部署创建 [监视规则](/graph/api/resources/windowsupdates-monitoringsettings)。 每个 [部署](/graph/api/resources/windowsupdates-deployments) 一次可以有一个活动的监视规则。

监视规则由三个部分组成：
* **signal**：部署服务要监视的更新问题的类型。
* **threshold：** 当此百分比的设备发出指定信号时，将触发监视规则。
* **action：** 触发监视规则时要执行的操作。

下面是在创建部署的同时为部署创建监视规则的示例。

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
                    "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
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
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-2-unpause-a-deployment-that-was-paused-by-a-monitoring-rule"></a>步骤 2：取消使用由监视规则暂停的部署
当监视规则触发时，它将有机会调查可能导致应用更新的更新问题。 调查后，你可能希望恢复部署。 有两种方法可以这样做：删除监视规则或更新监视规则阈值。

### <a name="example-resume-deployment-by-removing-a-monitoring-rule"></a>示例：通过删除监视规则恢复部署
触发暂停部署的监视规则时，恢复部署的一种方式是删除该规则。

下面是通过删除规则恢复部署的示例。

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
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

### <a name="example-resume-deployment-by-updating-a-monitoring-rule-threshold"></a>示例：通过更新监视规则阈值恢复部署
恢复部署的另一种方式是更改相关监视规则的阈值。 当达到新阈值时， (，) `pauseDeployment` 将再次触发操作。 

下面是通过更改监视规则阈值恢复部署的示例。 此示例还说明如何编辑任何现有的监视规则（即使尚未达到其阈值）以及如何在没有监控规则的部署上创建监视规则。

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
                    "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
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
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```
