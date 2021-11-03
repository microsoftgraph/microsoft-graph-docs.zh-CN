---
title: 使用 Windows Update for Business 部署服务管理安全措施
description: 使用部署服务部署更新时，该服务会自动保护部署，防止由 Windows 更新向具有已知或可能问题的设备提供更新。
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 22ce9a2e9e418ee5846881e72b98d213d9294247
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697014"
---
# <a name="manage-safeguards-using-the-windows-update-for-business-deployment-service"></a>使用 Windows Update for Business 部署服务管理安全措施

使用部署服务部署更新时，该服务会自动保护部署，防止由 Windows 更新向具有已知或可能问题的设备提供更新。

安全措施与部署[Windows 11](windowsupdates-deployments.md)和 Windows 10 功能更新兼容。 针对已知问题的保留可用于部署 Windows 11 和 Windows 10 功能更新，并可以针对部署 Windows 11 时可能的问题进行Windows 11。

## <a name="apply-all-safeguards"></a>应用所有安全措施

默认情况下，部署服务将所有适用的安全措施应用于部署中的设备。 若要从安全措施中获益，在创建部署时无需指定任何其他内容。

以下示例演示了如何创建应用所有安全措施的部署。

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

## <a name="opt-out-of-safeguards-against-likely-issues"></a>选择退出针对可能问题的安全措施

通过配置安全措施，可以选择退出针对部署中可能的问题 [的安全措施](/graph/api/resources/windowsupdates-safeguardsettings)。 如有必要，您还可以通过使用禁用安全措施策略选择退出对已知问题的 [安全措施](/windows/deployment/update/safeguard-opt-out)保留。

以下示例演示了如何创建部署，而不对可能的问题进行安全措施。 通过为要禁用的安全措施配置文件列表下的类别指定 **safeguardProfile，** 可将部署配置为向设备提供更新，即使设备可能出现更新 `likelyIssues` 问题。

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
