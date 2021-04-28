---
title: 删除 azureADDevice
description: 删除 azureADDevice 对象。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 6cb9d23b01241878eff96e7301f8322baa7f0fb0
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067841"
---
# <a name="delete-azureaddevice"></a>删除 azureADDevice
命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 对象。

删除 Azure AD 设备后，它将从部署服务注销，并自动注销该服务管理的所有更新类别，以及从每个 [deploymentAudience](../resources/windowsupdates-deploymentaudience.md) 和 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)中删除。

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
DELETE /admin/windows/updates/updatableAssets/{azureADDeviceId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "delete_azureaddevice"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{azureADDeviceId}
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

