---
title: deploymentAudience：updateAudienceById
description: 使用相同类型的 updatableAsset 资源更新 deploymentAudience 的成员和排除集合。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 1b948e644628eedc08fe470641b612501dfb80af
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351116"
---
# <a name="deploymentaudience-updateaudiencebyid"></a>deploymentAudience：updateAudienceById

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用相同类型的[updatableAsset](../resources/windowsupdates-updatableasset.md)资源更新[deploymentAudience](../resources/windowsupdates-deploymentaudience.md)的成员和排除集合。

向部署访问群体的成员或排除集合添加 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 会自动创建 Azure AD 设备对象（如果该对象不存在）。

如果 **deploymentAudience** 的排除和 **成员** 集合中包含相同的 [updatableAsset，](../resources/windowsupdates-updatableasset.md)则部署不会应用于该资产。 

您还可以使用 [updateAudience](windowsupdates-deploymentaudience-updateaudience.md) 方法来更新 **deploymentAudience**。

> [!NOTE]
> 此 API 具有 [与](/Graph/known-issues#accessing-and-updating-deployment-audiences) 通过 Intune 创建的部署相关的已知问题。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|WindowsUpdates.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|WindowsUpdates.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments/{deploymentId}/audience/updateAudienceById
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
|memberEntityType|字符串|可更新资源的完整类型。 可取值为：`#microsoft.graph.windowsUpdates.azureADDevice`、`#microsoft.graph.windowsUpdates.updatableAssetGroup`。|
|addMembers|String collection|与要添加为部署访问群体成员的可更新资产对应的标识符列表。|
|removeMembers|String collection|与要作为部署访问群体成员删除的可更新资源相对应的标识符列表。|
|addExclusions|String collection|与要作为部署访问群体排除项添加的可更新资源相对应的标识符列表。|
|removeExclusions|String collection|与要作为部署访问群体排除项删除的可更新资源相对应的标识符列表。|



## <a name="response"></a>响应

如果成功，此操作返回 `202 Accepted` 响应代码。 它不会在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "deploymentaudience_updateaudiencebyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/updateAudienceById
Content-Type: application/json
Content-length: 204

{
  "memberEntityType": "String",
  "addMembers": [
    "String"
  ],
  "removeMembers": [
    "String"
  ],
  "addExclusions": [
    "String"
  ],
  "removeExclusions": [
    "String"
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/deploymentaudience-updateaudiencebyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/deploymentaudience-updateaudiencebyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/deploymentaudience-updateaudiencebyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/deploymentaudience-updateaudiencebyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

