---
title: 列出可更新资源组的成员
description: 列出 updatableAssetGroup 资源的成员。 成员为 azureADDevice 类型。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: d4e4ffca528bd4e66b0a407fe14f42a8198aa913
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067837"
---
# <a name="list-updatable-asset-group-members"></a>列出可更新资源组的成员
命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

列出 [updatableAssetGroup 资源](../resources/windowsupdates-updatableassetgroup.md) 的成员。 成员为 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 类型。

此操作引用 **updatableAssetGroup** 资源的 members 导航属性。  若要引用派生自 [updatableAsset](../resources/windowsupdates-updatableasset.md)的类型的属性，在查询 URL 中包括完全派生的资源类型，即 `.../microsoft.graph.windowsUpdates.updatableAssetGroup/members` 。

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
GET /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/microsoft.graph.windowsUpdates.updatableAssetGroup/members
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 [OData 查询](/graph/query-parameters) 参数来帮助自定义响应，包括 `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。

若要对不是从 [updatableAsset](../resources/windowsupdates-updatableasset.md)继承的属性使用查询参数，请包含属性的完整资源类型。 例如，若要应用于 `$select` [azureADDevice](../resources/windowsupdates-azureaddevice.md)的 **errors** 属性，请使用 `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` 。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [updatableAsset](../resources/windowsupdates-updatableasset.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/microsoft.graph.windowsUpdates.updatableAssetGroup/members
```


### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.updatableAsset)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "f5ba7065-7065-f5ba-6570-baf56570baf5"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "6d49dfaf-9c24-42f7-9628-c136e35774c8"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "1f61492e-4e34-4dee-904a-0d38299e76b2"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "bfe3c2d1-4cef-4952-8c5e-30d56ccf0cdc"
    }
  ]
}
```

