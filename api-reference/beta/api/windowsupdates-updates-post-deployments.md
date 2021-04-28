---
title: 创建部署
description: 创建新的部署对象。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 5c2b9c4a228aa33b7bf5ff134a43b265a8e01486
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067318"
---
# <a name="create-deployment"></a>创建部署
命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> [!NOTE]
> 如果在创建 [部署时未指定](/graph/api/resources/windowsupdates-monitoringrule) 监视规则，则创建默认监视规则。 此默认监视规则具有 **信号**、阈值 和 `rollback`  `20` **操作** `alertError` 。 在 API 的未来更新中，此行为将更改，并且不会创建默认监视规则。

创建新的 [部署](../resources/windowsupdates-deployment.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|WindowsUpdates.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|WindowsUpdates.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供部署对象的 JSON [表示](../resources/windowsupdates-deployment.md) 形式。

下表显示创建部署时所需的 [属性](../resources/windowsupdates-deployment.md)。

|属性|类型|说明|
|:---|:---|:---|
|内容|[microsoft.graph.windowsUpdates.deployableContent](../resources/windowsupdates-deployablecontent.md)|指定要部署的内容。 应作为以下派生类型之一提供可部署内容[：expeditedQualityUpdateReference、featureUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md) [](../resources/windowsupdates-featureupdatereference.md)|



## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应[](../resources/windowsupdates-deployment.md)代码和部署对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_deployment_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments
Content-Type: application/json
Content-length: 344

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "content": {
    "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
    "version": "20H2"
  },
  "settings": {
    "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
    "rollout": {
      "devicesPerOffer": 100
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

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
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

