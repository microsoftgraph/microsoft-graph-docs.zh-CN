---
title: 使用 Windows Update for Business 部署服务安排部署
description: 使用部署服务部署更新时，可以计划部署，以便设备在未来日期接收更新。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 650e35dc8496bcb9e2dbcee33d7dfca58db1615b
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61854826"
---
# <a name="schedule-a-deployment-using-the-windows-update-for-business-deployment-service"></a>使用 Windows Update for Business 部署服务安排部署

使用部署服务部署更新时，可以计划部署，以便设备在未来日期接收更新。

计划功能与部署[功能Windows 10](windowsupdates-deployments.md)兼容。

## <a name="schedule-a-deployment-to-start-at-a-future-date"></a>计划部署在未来日期开始

可以通过配置部署设置，计划部署在未来日期 [开始](/graph/api/resources/windowsupdates-rolloutsettings)。 在下面的示例中，分配了部署的所有设备都将在 2021 年 7 月 1 日获得更新。

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

## <a name="stage-a-deployment-over-a-period-of-time"></a>在一段时间内部署阶段

还可以计划部署，以便向分配的设备提供逐步推出中的更新，该部署会逐步进行。 更新按固定间隔提供给分配到部署的设备的子集，推出的总持续时间由结束日期或产品/服务费率决定。 可以将逐步推出视为类似于定期日历事件系列。

### <a name="example-stage-a-deployment-at-regular-intervals-between-start-and-end-dates"></a>示例：在开始日期和结束日期之间定期部署

在一定时间阶段部署一种方式是设置部署的 **endDateTime。** 分配给部署的所有设备都将在 **startDateTime** 和 **endDateTime** 之间的窗口中提供更新。 如果 **未指定 startDateTime，** 则分配设备后将立即开始部署。

本示例将配置新的部署，以便从 2021 年 7 月 1 日开始，每周向一组新设备提供更新 (**durationBetweenOffers** 设置为) 年 7 天。 在 2021 年 8 月 1 日之前，会向所有设备提供更新。

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


### <a name="example-stage-a-deployment-at-regular-intervals-with-a-specified-number-of-devices-at-each-offer"></a>示例：定期部署，每个产品/服务具有指定数量的设备

在一段时间后部署阶段的另一种方式是使用 配置产品/服务费率 `devicesPerOffer` 。 分配给部署的设备将按照指定的速率提供更新，直到所有设备都获得更新。

本示例将配置新的部署，以便从 2021 年 7 月 1 日开始，每周向一组新设备提供更新 (**durationBetweenOffers** 设置为) 年 7 天。 一次向 100 台设备提供更新，直到所有设备都获得更新。

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
