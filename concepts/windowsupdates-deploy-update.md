---
title: 使用 Windows Update for Business 部署服务部署功能更新
description: 使用 Windows Update for Business 部署服务，Windows Azure AD 租户中的设备部署功能更新。
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 9bc32b4f49a2cb985d1b19f49e72d2c373bb4e6e
ms.sourcegitcommit: 11be55b40804b07f4c422f09f601afa97c7d31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2021
ms.locfileid: "60255939"
---
# <a name="deploy-a-feature-update-using-the-windows-update-for-business-deployment-service"></a>使用 Windows Update for Business 部署服务部署功能更新

使用 Windows Update for Business 部署服务，Windows Azure AD 租户中的设备部署更新。 如今，部署服务[支持部署Windows 10](windowsupdates-deployments.md)更新和加速安全更新。 本主题重点介绍功能更新的部署。 有关部署快速安全更新的信息，请参阅 [D部署加速安全更新](windowsupdates-deploy-expedited-update.md)。

将功能更新部署到设备时，Windows更新会向设备提供指定的更新（如果设备尚未收到更新）。 例如，如果将 Windows 10 功能更新版本 20H2 部署到已注册功能更新管理且当前位于较旧版本的 Windows 10 的设备，则设备将更新到版本 20H2。 如果设备已位于或高于 20H2 版本，它将保持其当前版本。 如果设备未注册功能更新管理，则此操作不会影响设备。

只要设备仍在功能更新管理中注册，设备就不会从 Windows Update 接收任何其他功能更新，除非使用部署服务显式部署。

> [!IMPORTANT]
> 通过使用 Windows Update for Business 部署服务将设备升级到 Windows 11 (，将部署的版本参数设置为"Windows 11， 版本 21H2") ，你同意在将此操作系统应用于设备时， (1) 通过批量许可购买了适用的 Windows 许可证，或你有权购买的 (2) 绑定你的组织并代表其接受相关 Microsoft 软件许可条款，可在此处找到[：Microsoft 软件许可条款](https://www.microsoft.com/Useterms)。

## <a name="prerequisites"></a>先决条件

* 设备满足 [部署服务的先决条件](windowsupdates-concept-overview.md#prerequisites)。
* 在可以使用部署服务部署功能更新之前，设备必须由功能更新类别的部署服务[](windowsupdates-enroll.md)在管理中注册。

## <a name="step-1-optional-get-a-list-of-deployable-updates"></a>步骤 1： (可选) 获取可部署更新的列表

你可以查询部署服务目录，获取可以部署中的内容部署到设备的更新列表。

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

[部署](/graph/api/resources/windowsupdates-deployment)指定要部署的内容、如何以及何时部署内容以及目标设备。 创建部署后，将自动将部署访问群体创建为关系。

下面是使用配置部署计划及监视规则的可选设置创建功能[更新部署](windowsupdates-schedule-deployment.md)[的示例](windowsupdates-manage-monitoring-rules.md)。 目标设备在下一步中指定。

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
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-3-assign-devices-to-the-deployment-audience"></a>步骤 3：将设备分配给部署访问群体

创建部署后，你可以将设备分配给部署 [访问群体](/graph/api/resources/windowsupdates-deploymentaudience)。 成功更新部署访问群体后，Windows更新开始根据部署设置向相关设备提供更新。

在将设备添加到部署访问群体的成员或排除集合时 (会自动向服务注册设备 (也就是说，如果 [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) 对象) 。

以下示例演示如何将 Azure AD 设备添加为部署访问群体的成员。

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

在部署过程中，可以通过更新部署的状态来暂停部署，也可以更新其访问群体成员和排除项。

## <a name="after-a-deployment"></a>部署后

在最初向部署访问群体分配的所有设备都提供更新后，由于设备连接等因素，并非所有设备都启动或完成了更新。 只要部署仍然存在，Windows只要重新连接，更新就会继续为分配的设备提供更新。

