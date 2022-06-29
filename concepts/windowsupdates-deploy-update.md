---
title: 使用 Windows 更新 for Business 部署服务部署功能更新
description: 按照以下步骤，使用 Windows 更新 for Business 部署服务将 Windows 功能更新部署到 Azure AD 租户中的设备。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 176d4c07348b367bfe02335617ebae3328573907
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437504"
---
# <a name="deploy-a-feature-update-using-the-windows-update-for-business-deployment-service"></a>使用 Windows 更新 for Business 部署服务部署功能更新

使用 Windows 更新 for Business 部署服务，可以将 Windows 更新部署到 Azure AD 租户中的设备。 目前，部署服务支持[部署](windowsupdates-deployments.md)Windows 10功能更新和加速安全更新。 本主题重点介绍功能更新的部署。 有关部署加速安全更新的信息，请 [参阅部署加速的安全更新](windowsupdates-deploy-expedited-update.md)。

将功能更新部署到设备时，如果设备尚未收到更新，Windows 更新会向设备提供指定的更新。 例如，如果将Windows 10功能更新版本 20H2 部署到已在功能更新管理中注册且当前处于较旧版本Windows 10的设备，则设备将更新到版本 20H2。 如果设备已在版本 20H2 或更高版本中，则保持其当前版本。 如果设备未在功能更新管理中注册，则设备不受此操作的影响。

只要设备仍注册在功能更新管理中，设备就不会从Windows 更新接收任何其他功能更新，除非使用部署服务显式部署。

> [!IMPORTANT]
> 通过使用 Windows 更新 for Business 部署服务将设备升级到Windows 11 (，将部署的版本参数设置为“Windows 11版本 21H2”) ，你同意在将此操作系统应用于设备时， (1) 通过批量许可购买适用的 Windows 许可证，或者 (2) ，你有权绑定你的 组织并代表其接受此处要找到的相关 Microsoft 软件许可[条款：Microsoft 软件许可条款](https://www.microsoft.com/Useterms)。

## <a name="prerequisites"></a>先决条件

* 设备满足 [部署服务的先决条件](windowsupdates-concept-overview.md#prerequisites)。
* 在使用部署服务部署功能更新之前，必须由功能更新类别的部署服务 [在管理中注册](windowsupdates-enroll.md) 设备。

## <a name="step-1-optional-get-a-list-of-deployable-updates"></a>步骤 1： (可选) 获取可部署更新的列表

可以查询部署服务目录以获取可作为部署内容部署到设备的更新列表。

下面是查询部署服务可部署的所有Windows 10功能更新的示例。

### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/catalog/entries?$filter=isof('microsoft.graph.windowsUpdates.featureUpdateCatalogEntry')
```

### <a name="response"></a>响应

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
            "id": "560a186a-1434-4364-8330-deb944b494ff",
            "displayName": "Windows 10, version 20H2",
            "releaseDate": "String (timestamp)",
            "deployableUntilDateTime": "String (timestamp)",
            "version": "20H2"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
            "id": "5e436dae-56bd-4925-bf8b-acf550e07227",
            "displayName": "Windows 10, version 2004",
            "releaseDate": "String (timestamp)",
            "deployableUntilDateTime": "String (timestamp)",
            "version": "2004"
        }
    ]
}
```

## <a name="step-2-create-a-deployment"></a>步骤 2：创建部署

[部署](/graph/api/resources/windowsupdates-deployment)指定要部署的内容、部署内容的方式和时间以及目标设备。 创建部署时，会自动创建部署受众作为关系。

下面是创建功能更新部署的示例，其中包含配置 [部署计划](windowsupdates-schedule-deployment.md) 和 [监视规则](windowsupdates-manage-monitoring-rules.md)的可选设置。 默认情况下应用[安全措施](windowsupdates-manage-safeguards.md)。 目标设备在下一步中指定。

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
            "devicesPerOffer": 100,
            "durationBetweenOffers": "P7D"
        },
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
        "rollout": {
            "devicesPerOffer": 100,
            "durationBetweenOffers": "P7D",
            "startDateTime": null,
            "endDateTime": null
        },
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
        "safeguard": null,
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-3-assign-devices-to-the-deployment-audience"></a>步骤 3：将设备分配给部署受众

创建部署后，可以将设备分配给 [部署受众](/graph/api/resources/windowsupdates-deploymentaudience)。 成功更新部署受众后，Windows 更新开始根据部署设置向相关设备提供更新。

设备在添加到部署受众的成员或排除项集合时自动注册到服务， (即，如果) 尚不存在，则会自动创建 [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) 对象。

以下示例演示如何将 Azure AD 设备添加为部署受众的成员。

### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
Content-type: application/json

{
    "addMembers": [
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
            "id": "String (identifier)"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
            "id": "String (identifier)"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
            "id": "String (identifier)"
        }
    ]
}
```

### <a name="response"></a>响应

```http
HTTP/1.1 202 Accepted
```

## <a name="during-a-deployment"></a>部署期间

部署正在进行时，可以通过更新部署 **的状态** 以及更新其受众成员和排除项来暂停部署。

## <a name="after-a-deployment"></a>部署后

分配给部署受众的所有设备最初都已提供更新后，由于设备连接等因素，可能并非所有设备都已启动或完成更新。 只要部署仍然存在，Windows 更新只要重新连接，就会继续向分配的设备提供更新。

