---
title: 使用 Windows 更新 for Business 部署服务管理安全措施
description: 使用 Windows 更新 for Business 部署服务部署更新时，它会自动阻止有问题的设备提供更新。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 5373fe27415bbfd552303e7d154be131bdf76e11
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437441"
---
# <a name="manage-safeguards-using-the-windows-update-for-business-deployment-service"></a>使用 Windows 更新 for Business 部署服务管理安全措施

使用部署服务部署更新时，该服务会通过阻止Windows 更新提供已知或可能出现问题的设备来自动保护部署。

安全措施与Windows 11和Windows 10功能更新的[部署](windowsupdates-deployments.md)兼容。 针对已知问题的保护措施可用于部署Windows 11和Windows 10功能更新，并针对部署Windows 11时可能出现的问题进行保护。

## <a name="apply-all-safeguards"></a>应用所有安全措施

默认情况下，部署服务将所有适用的保障措施应用到部署中的设备。 若要受益于安全措施，无需在创建部署时指定任何其他内容。

以下示例演示如何创建应用了所有安全措施的部署。

### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
        "version": "20H2"
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
    "settings": null,
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="opt-out-of-safeguards-against-likely-issues"></a>选择退出针对可能出现的问题的安全措施

通过配置安全设置，可以选择退出针对部署中可能出现的问题 [的防护](/graph/api/resources/windowsupdates-safeguardsettings)措施。 如有必要，还可以通过 [使用禁用保障措施策略，选择退出已知问题的保护](/windows/deployment/update/safeguard-opt-out)保留。

以下示例演示如何创建部署，而无需针对可能出现的问题提供保障。 通过为要禁用的保护配置文件列表下的`likelyIssues`**类别** 指定 **一个 safeguardProfile**，你将部署配置为向设备提供更新，即使它可能存在更新问题。

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
        "safeguard": {
            "disabledSafeguardProfiles": [
                {
                    "category": "likelyIssues"
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
        "monitoring": null,
        "rollout": null,
        "userExperience": null,
        "safeguard": {
            "disabledSafeguardProfiles": [
                {
                    "@odata.type": "#microsoft.graph.windowsUpdates.safeguardProfile",
                    "category": "likelyIssues"
                }
            ]
        }
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```
