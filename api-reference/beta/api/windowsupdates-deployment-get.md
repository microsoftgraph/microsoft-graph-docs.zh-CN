---
title: 获取部署
description: 读取部署对象的属性和关系。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 43081598030efc8ac4b3e30fe35d99931dde5d8f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067840"
---
# <a name="get-deployment"></a>获取部署
命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取部署 [对象的属性和](../resources/windowsupdates-deployment.md) 关系。

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
GET /admin/windows/updates/deployments/{deploymentId}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应[](../resources/windowsupdates-deployment.md)代码和部署对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_deployment"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
```


### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "id": "b5171742-1742-b517-4217-17b5421717b5",
    "state": {
      "@odata.type": "microsoft.graph.windowsUpdates.deploymentState"
    },
    "content": {
      "@odata.type": "microsoft.graph.windowsUpdates.deployableContent"
    },
    "settings": {
      "@odata.type": "microsoft.graph.windowsUpdates.deploymentSettings"
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
  }
}
```

