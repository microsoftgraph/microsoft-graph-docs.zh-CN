---
title: 列出 riskyUsers
description: 获取 riskyUser 对象及其属性的列表。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dd6d413803e7461ffe0f00891b6e4db7cd3d0e0b
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897552"
---
# <a name="list-riskyusers"></a>列出 riskyUsers
命名空间：microsoft.graph

获取[riskyUser](../resources/riskyuser.md)对象及其属性的列表。

## <a name="permissions"></a>权限
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户） | IdentityRiskyUser.Read.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | IdentityRiskyUser.Read.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 OData 查询参数来帮助自定义响应。 有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[riskyUser](../resources/riskyuser.md)对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers
```


### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.riskyUser)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.riskyUser",
      "id": "d1d4a5d4-a5d4-d1d4-d4a5-d4d1d4a5d4d1",
      "isDeleted": "Boolean",
      "isProcessing": "Boolean",
      "riskLastUpdatedDateTime": "String (timestamp)",
      "riskLevel": "String",
      "riskState": "String",
      "riskDetail": "String",
      "userDisplayName": "String",
      "userPrincipalName": "String"
    }
  ]
}
```

