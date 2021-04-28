---
title: deploymentAudience：updateAudience
description: 更新 deploymentAudience 的成员和排除集合。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: a0567070f4042896835b735fa69b5cd1dddeb1a3
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067337"
---
# <a name="deploymentaudience-updateaudience"></a>deploymentAudience：updateAudience
命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [deploymentAudience](../resources/windowsupdates-deploymentaudience.md)的成员和排除集合。

向部署访问群体的成员或排除集合添加 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 会自动创建 Azure AD 设备对象（如果该对象不存在）。

如果 **deploymentAudience** 的排除和 **成员** 集合中包含相同的 [updatableAsset，](../resources/windowsupdates-updatableasset.md)则部署不会应用于该资产。 

如果 **所有 updatableAsset** 对象都是同一类型，则也可使用 [updateAudienceById](windowsupdates-deploymentaudience-updateaudiencebyid.md) 方法更新 **deploymentAudience**。

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
POST /admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|说明|
|:---|:---|:---|
|addMembers|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合|要添加为部署访问群体成员的 [updatableAsset](../resources/windowsupdates-updatableasset.md) 资源的列表。|
|removeMembers|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合|要作为部署访问群体成员删除的可更新资源的列表。|
|addExclusions|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合|要添加为部署访问群体排除项的可更新资源列表。|
|removeExclusions|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合|要作为部署访问群体排除项删除的可更新资源的列表。|



## <a name="response"></a>响应

如果成功，此操作返回 `202 Accepted` 响应代码。 它不会在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "deploymentaudience_updateaudience"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
Content-Type: application/json
Content-length: 599

{
  "addMembers": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ],
  "removeMembers": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ],
  "addExclusions": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ],
  "removeExclusions": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ]
}
```


### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

