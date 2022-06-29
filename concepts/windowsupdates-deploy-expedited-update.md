---
title: 使用 Windows 更新 for Business 部署服务部署加速的安全更新
description: 在发生紧急情况时，请按照以下步骤使用 Windows 更新 for Business 部署服务，将快速 Windows 安全更新部署到 Azure AD 租户中的设备。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: c0c8d0389c2d152ebc4323639c0b8494927f89e7
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444213"
---
# <a name="deploy-an-expedited-security-update-using-the-windows-update-for-business-deployment-service"></a>使用 Windows 更新 for Business 部署服务部署加速的安全更新

使用 Windows 更新 for Business 部署服务，可以将 Windows 更新部署到 Azure AD 租户中的设备。 目前，部署服务支持[部署](windowsupdates-deployments.md)Windows 10功能更新和加速安全更新。 本主题重点介绍加速安全更新的部署。 有关部署功能更新的信息，请参阅 [“部署功能更新](windowsupdates-deploy-update.md)”。

加速安全更新将替代业务延迟策略的Windows 更新，以便尽快安装更新。 当出现关键安全事件并且需要比正常部署最新更新更快时，它可以非常有用。 但是，尽管它可以帮助实现针对特定安全更新的符合性目标，但并不是每个月都使用它。 请考虑使用 [符合性截止时间进行更新](/windows/deployment/update/wufb-compliancedeadlines)。

将加速安全更新部署到设备时，如果设备尚未收到具有指定发布日期的更新，Windows 更新会向设备提供最新的适用更新。 例如，如果将 2021 年 4 月 13 日发布的Windows 10安全更新部署到当前没有更新的设备，则设备将收到加速更新。 如果设备已具有指定的更新或更新，则不会收到加速更新。

快速安全更新还具有以下特征：

* 更新立即启动，而不是等待下一次定期更新扫描，默认情况下每 22 小时进行一次。
* 更新将尽快下载和安装。
* 更新过程会覆盖配置的设备策略设置，例如，在设备被强制重启之前几天。 安装快速更新后，设备将返回到当前策略设置。

## <a name="prerequisites"></a>先决条件

* 设备满足 [部署服务的先决条件](windowsupdates-concept-overview.md#prerequisites)。
* 设备已安装 [KB4023057 中所述的更新 - 更新Windows 10更新服务组件](https://support.microsoft.com/topic/kb4023057-update-for-windows-10-update-service-components-fccad0ca-dc10-2e46-9ed1-7e392450fb3a) (或更新) 。

## <a name="step-1-optional-get-a-list-of-expeditable-updates"></a>步骤 1： (可选) 获取可快速更新的列表

可以查询部署服务目录，以获取可作为部署内容加速到设备的更新列表。

安全更新由 [qualityUpdateCatalogEntry](/graph/api/resources/windowsupdates-qualityupdatecatalogentry) 类型表示，**其质量为 QualityUpdateClassification**`security`。 所有归类为安全更新的Windows 10质量更新都可以加速，并使用 **isExpeditable** 属性设置为标`true`识它们进行标记。

下面是查询部署服务可作为加速更新部署的所有Windows 10安全更新的示例。 Microsoft 建议仅显示三个最新的更新，因此该示例包括 `$top=3`。

### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/catalog/entries?$top=3&$filter=isof('microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry') and microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry/isExpeditable eq true&$orderby=releaseDateTime desc
```

### <a name="response"></a>响应

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
            "id": "bd9554dc-2737-4e3c-b794-fa2b8b3f4a30",
            "displayName": "MM/DD/YYYY - YYYY.MM B Security Updates for Windows 10",
            "releaseDateTime": "String (timestamp)",
            "deployableUntilDateTime": null,
            "isExpeditable": true,
            "qualityUpdateClassification": "security"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
            "id": "68860630-c2d0-4dd2-8c4b-9b9737ee5081",
            "displayName": "MM/DD/YYYY - YYYY.MM B Security Updates for Windows 10",
            "releaseDateTime": "String (timestamp)",
            "deployableUntilDateTime": null,
            "isExpeditable": true,
            "qualityUpdateClassification": "security"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
            "id": "aa336b13-db33-4d94-89ea-90e43e4ad30b",
            "displayName": "MM/DD/YYYY - YYYY.MM B Security Updates for Windows 10",
            "releaseDateTime": "String (timestamp)",
            "deployableUntilDateTime": null,
            "isExpeditable": true,
            "qualityUpdateClassification": "security"
        }
    ]
}
```

## <a name="step-2-create-a-deployment"></a>步骤 2：创建部署

[部署](/graph/api/resources/windowsupdates-deployment)指定要部署的内容、部署内容的方式和时间以及目标设备。 对于质量更新，内容是使用目标符合性日期指定的。 创建部署时，会自动创建部署受众作为关系。

将加速安全更新部署到设备时，Windows 更新提供更新，使设备高于指定的最低符合性级别。 根据每个设备扫描和更新的时间，某些设备可能会收到较新的更新 (例如，如果有比所需最低符合性级别) 对应的更新更新的安全更新，但所有设备都符合指定的安全更新符合性标准。 提供最新适用更新的行为（由属性 **等效的Content** 设置为默认值 `latestSecurity`所指示）有助于尽可能保护设备的安全，并防止设备在几天后收到加速更新，然后再收到另一个常规更新。

可以在部署的 [用户体验设置](/graph/api/resources/windowsupdates-userexperiencesettings)中使用属性 **daysUntilForcedReboot** 配置设备重启宽限期。 宽限期设置安装后用户可以控制设备重启时间的时间。 如果设备在宽限期到期时尚未重启，则会自动重启。

下面是为加速质量更新创建部署的示例。 目标设备在下一步中指定。

### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.expeditedQualityUpdateReference",
        "releaseDate": "YYYY-MM-DD"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "userExperience": {
            "daysUntilForcedReboot": 2
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
        "@odata.type": "microsoft.graph.windowsUpdates.expeditedQualityUpdateReference",
        "releaseDate": "YYYY-MM-DDT00:00:00Z",
        "classification": "security",
        "equivalentContent": "latestSecurity"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "userExperience": {
            "daysUntilForcedReboot": 2
        },
        "monitoring": null,
        "rollout": null,
        "safeguard": null
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

分配给部署受众的所有设备最初都已提供更新后，由于设备连接等因素，可能并非所有设备都已启动或完成更新。 只要部署仍然存在，它就会继续确保Windows 更新每次重新连接时都会向分配的设备提供更新。
