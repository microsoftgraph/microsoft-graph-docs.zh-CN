---
title: updatableAsset：unenrollAssetsById
description: 从部署服务的更新管理中注销相同类型的 UpdatableAsset 资源。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 8e738a6ecfcf5f6a11e2433f20c784d53fc8eedd
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067326"
---
# <a name="updatableasset-unenrollassetsbyid"></a>updatableAsset：unenrollAssetsById
命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从部署服务的更新管理中注销相同类型的 [UpdatableAsset](../resources/windowsupdates-updatableasset.md) 资源。

您还可以使用 [unenrollAssets 方法](windowsupdates-updatableasset-unenrollassets.md) 注销资产。

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
POST /admin/windows/updates/updatableAssets/unenrollAssetsById
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
|updateCategory|microsoft.graph.windowsUpdates.updateCategory|要停止管理的服务的更新类别。 支持 **updateCategory** 值的子集。 可能的值是 `feature` ：。|
|memberEntityType|String|**updatableAsset 资源的完整** 类型。 可能的值是 `#microsoft.graph.windowsUpdates.azureADDevice` ：。|
|ids|String collection|与 **updatableAsset** 资源对应的标识符列表，用于注销给定 **updateCategory** 的服务的更新管理。|

## <a name="response"></a>响应

如果成功，此操作返回 `202 Accepted` 响应代码。 它不会在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "updatableasset_unenrollassetsbyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/unenrollAssetsById
Content-Type: application/json

{
  "updateCategory": "feature",
  "memberEntityType": "#microsoft.graph.windowsUpdates.azureADDevice",
  "ids": [
    "String",
    "String",
    "String"
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

