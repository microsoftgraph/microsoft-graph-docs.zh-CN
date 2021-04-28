---
title: updatableAsset：unenrollAssets
description: 从部署服务的更新管理中注销 updatableAsset 资源。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 3e714d403fdc6423053bd958201abd3e95352f0f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067329"
---
# <a name="updatableasset-unenrollassets"></a>updatableAsset：unenrollAssets
命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从部署服务的更新管理中注销 [updatableAsset](../resources/windowsupdates-updatableasset.md) 资源。

您还可以使用 [unenrollAssetsById](windowsupdates-updatableasset-unenrollassetsbyid.md) 方法注销资产。

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
POST /updatableAssetGroup/members/unenrollAssets
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
|assets|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合|要从服务的更新管理中注销的 **updatableAsset** 资源列表，用于给定 **updateCategory**。|



## <a name="response"></a>响应

如果成功，此操作返回 `202 Accepted` 响应代码。 它不会在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "updatableasset_unenrollassets"
}
-->
``` http
POST https://graph.microsoft.com/beta/updatableAssetGroup/members/unenrollAssets
Content-Type: application/json

{
  "updateCategory": "String",
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
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

