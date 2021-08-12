---
title: 使用 Windows Update for Business 部署服务部署快速安全更新
description: 借助 Windows Update for Business 部署服务，你可以将加速 Windows 安全更新部署到 Azure AD 租户中的设备，以防出现紧急情况，并需要立即部署安全更新。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: ea65dc16cd45d4b5da2ba5c850e97fd662b39bedd02eb9502e970d789ca98d0b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54225662"
---
# <a name="deploy-an-expedited-security-update-using-the-windows-update-for-business-deployment-service"></a>使用 Windows Update for Business 部署服务部署快速安全更新

使用 Windows Update for Business 部署服务，Windows Azure AD 租户中的设备部署更新。 如今，部署服务[支持部署](windowsupdates-deployments.md)Windows 10更新和加速安全更新。 本主题重点介绍快速安全更新的部署。 有关部署功能更新的信息，请参阅 [部署功能更新](windowsupdates-deploy-update.md)。

安装安全更新会覆盖Windows更新的延迟策略，以便尽快安装更新。 当出现关键安全事件并且需要比正常情况更快速地部署最新更新时，它非常有用。 但是，虽然它可以帮助实现针对特定安全更新的合规性目标，但它并非旨在每月使用一次。 相反，请考虑使用 [更新的合规性截止时间](https://docs.microsoft.com/windows/deployment/update/wufb-compliancedeadlines)。

将加速安全更新部署到设备时，Windows更新会向设备提供最新的适用更新（如果设备尚未收到具有指定发布日期的更新）。 例如，如果将 2021 Windows 10 2021 年 4 月 13 日发布的更新安全更新部署到当前没有更新的设备，则设备将收到快速更新。 如果设备已具有指定的更新或更新版本，则它不会收到加速更新。

加速安全更新还具有以下特征：

* 更新立即启动，而不是等待下一次定期更新扫描，默认情况下每 22 小时进行一次。
* 更新将尽快下载和安装。
* 更新过程会覆盖配置的设备策略设置，例如，在设备被强制重启之前几天。 安装快速更新后，设备将返回到当前策略设置。

## <a name="prerequisites"></a>先决条件

* 设备满足 [部署服务的先决条件](windowsupdates-concept-overview.md#prerequisites)。
* 设备已安装[KB4023057 - Windows 10 Update Service](https://support.microsoft.com/topic/kb4023057-update-for-windows-10-update-service-components-fccad0ca-dc10-2e46-9ed1-7e392450fb3a)组件更新 (更新) 。

## <a name="step-1-optional-get-a-list-of-expeditable-updates"></a>步骤 1： (可选) 获取可安装更新的列表

你可以查询部署服务目录，获取更新列表，这些更新可以加速到设备作为部署中的内容。

安全更新由 [qualityUpdateCatalogEntry](/graph/api/resources/windowsupdates-qualityupdatecatalogentry) 类型表示 **，qualityUpdateClassification** 为 `security` 。 所有Windows 10分类为安全更新的更新质量更新都可以加速，并且使用设置为 的 **isExpeditable** 属性进行 `true` 标记以标识它们。

下面是一个查询所有 Windows 10 安全更新的示例，这些安全更新可通过部署服务作为快速更新进行部署。 Microsoft 建议只显示三个最新更新，因此该示例包括 `$top=3` 。

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

[部署](/graph/api/resources/windowsupdates-deployment)指定要部署的内容、如何以及何时部署内容以及目标设备。 对于质量更新，使用目标合规性日期指定内容。 创建部署后，将自动将部署访问群体创建为关系。

将加速安全更新部署到设备时，Windows更新会提供一个更新，将设备超过指定的最低合规性级别。 根据每个设备扫描和更新时间，某些设备可能会收到更新 (例如，如果有比所需最低合规性级别) 更新更新的更新，但所有设备都符合指定的安全更新合规性标准。 这种提供最新适用更新的行为（由设置为默认值的属性 **equivalentContent** 指示）有助于尽可能确保设备安全，并阻止设备在几天后收到快速更新，然后收到另一个 `latestSecurity` 定期更新。

可以使用部署用户体验设置中的 **属性 daysUntilForcedReboot** 配置 [设备重启](/graph/api/resources/windowsupdates-userexperiencesettings) 宽限期。 宽限期设置安装后用户可以控制设备重启时间的时间量。 如果设备在宽限期到期时尚未重新启动，则会自动重新启动。

下面是为快速质量更新创建部署的示例。 目标设备在下一步中指定。

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
        "rollout": null
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

在最初向部署访问群体分配的所有设备都提供更新后，由于设备连接等因素，并非所有设备都启动或完成了更新。 只要部署仍然存在，它就会继续确保Windows只要重新连接，就会向分配的设备提供更新。
