---
title: 列表快照
description: 获取 cloudPcSnapshot 对象及其属性的列表。
author: xintaozMS
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: b36c8a02b385a4ce0281fe2b3f3403f89b2ccf3d
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2022
ms.locfileid: "62879303"
---
# <a name="list-snapshots"></a>列表快照
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [cloudPcSnapshot 对象](../resources/cloudpcsnapshot.md) 及其属性的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|CloudPC.Read.All、CloudPC.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|CloudPC.Read.All、CloudPC.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/virtualEndpoint/snapshots
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 OData `$filter` 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [cloudPcSnapshot](../resources/cloudpcsnapshot.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

请求示例如下所示。

<!-- {
  "blockType": "request",
  "name": "list_cloudpcsnapshot"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/snapshots
```


### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcSnapshot",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcSnapshot",
      "cloudPcId": "662009bc-7732-4f6f-8726-25883518b33e",
      "createdDateTime": "2021-08-23T09:28:32.8260335Z",
      "lastRestoredDateTime": "2021-09-01T09:28:32.8260338Z",
      "id": "A00009UV000_93aff428-61f2-467f-a879-1102af6fd4a8",
      "status": "ready"
    }
  ]
}
```

