---
title: 使用 Windows 更新 for Business 部署服务计划部署
description: 部署更新时，可以计划部署，以便设备稍后使用 Windows 更新 for Business 部署服务接收更新。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 60d505eb5fab2ef003bb04762b6cccf3974e4f25
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437385"
---
# <a name="schedule-a-deployment-using-the-windows-update-for-business-deployment-service"></a>使用 Windows 更新 for Business 部署服务计划部署

使用部署服务部署更新时，可以计划部署，以便设备在将来的日期接收更新。

计划功能与Windows 10功能更新的[部署](windowsupdates-deployments.md)兼容。

## <a name="schedule-a-deployment-to-start-at-a-future-date"></a>计划部署以在将来的日期开始

可以通过配置部署 [的推出设置](/graph/api/resources/windowsupdates-rolloutsettings)，将部署安排在将来的日期开始。 在下面的示例中，分配了部署的所有设备将在 2021 年 7 月 1 日提供更新。

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
        "rollout": {
            "startDateTime": "2021-07-01T17:00:00Z",
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
        "rollout": {
            "startDateTime": "2021-07-01T17:00:00Z",
            "endDateTime": null,
            "durationBetweenOffers": "P1D",
            "devicesPerOffer": null
        },
        "monitoring": null,
        "userExperience": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="stage-a-deployment-over-a-period-of-time"></a>在一段时间内暂存部署

还可以计划部署，以便在随时间推移逐步推出时为分配的设备提供更新。 更新按常规时间间隔提供给分配给部署的设备子集，推出的总持续时间由结束日期或产品/服务速率决定。 可以将逐步推出视为类似于定期日历事件系列。

### <a name="example-stage-a-deployment-at-regular-intervals-between-start-and-end-dates"></a>示例：在开始日期和结束日期之间定期暂存部署

一种按时间分阶段部署的方法是设置部署的 **endDateTime** 。 分配给部署的所有设备都将在 **startDateTime** 和 **endDateTime** 之间的窗口中提供更新。 如果未指定 **startDateTime** ，则部署将在分配设备后立即开始。

在此示例中，你将配置新部署，以便从 2021 年 7 月 1 日开始，每周提供一组新设备， (**持续时间** 设置为 7 天) 。 所有设备都在 2021 年 8 月 1 日之前提供更新。

#### <a name="request"></a>请求

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
        "rollout": {
            "startDateTime": "2021-07-01T17:00:00Z",
            "endDateTime": "2021-08-01T17:00:00Z",
            "durationBetweenOffers": "P7D"
        }
    }
}
```

#### <a name="response"></a>响应

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
        "rollout": {
            "startDateTime": "2021-07-01T17:00:00Z",
            "endDateTime": "2021-08-01T17:00:00Z",
            "durationBetweenOffers": "P7D",
            "devicesPerOffer": null
        },
        "monitoring": null,
        "userExperience": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```


### <a name="example-stage-a-deployment-at-regular-intervals-with-a-specified-number-of-devices-at-each-offer"></a>示例：在每个产品/服务中按指定数量的设备定期进行部署

一段时间内进行部署的另一种方法是使用 `devicesPerOffer`>a0/a0> 配置产品/服务费率。 分配给部署的设备将按照指定的速率提供更新，直到所有设备都得到更新。

在此示例中，你将配置新部署，以便从 2021 年 7 月 1 日开始，每周提供一组新设备， (**持续时间** 设置为 7 天) 。 一次提供 100 台设备的更新，直到所有设备都获得更新。

#### <a name="request"></a>请求

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
        "rollout": {
            "startDateTime": "2020-07-01T17:00:00Z",
            "devicesPerOffer": 100,
            "durationBetweenOffers": "P7D"
        }
    }
}
```

#### <a name="response"></a>响应

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
        "rollout": {
            "startDateTime": "2020-07-01T17:00:00Z",
            "devicesPerOffer": 100,
            "durationBetweenOffers": "P7D",
            "endDateTime": null
        },
        "monitoring": null,
        "userExperience": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```
