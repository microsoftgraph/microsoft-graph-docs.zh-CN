---
title: 用户： exportPersonalData
description: 提交数据策略操作发出的请求，公司管理员通过导出组织用户的数据。
localization_priority: Normal
ms.openlocfilehash: d660994868e331fb8c1813bb9ff90aebe4790e9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845337"
---
# <a name="user-exportpersonaldata"></a>用户： exportPersonalData

提交数据策略操作发出的请求，由公司管理员导出组织用户的数据。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  User.Export.All 和 User.Read.All  |
|委派（个人 Microsoft 帐户） |  不适用  |
|应用程序 | User.Export.All 和 User.Read.All |

>**注意：** 使用委派的权限时，仅可由公司管理员执行导出。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a>请求标头
| 名称       | 说明 |
|:---------------|:----------|
| Authorization  | 持有者 {token}|

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |Description |
|:---------------|:--------|:----------|
|storageLocation|字符串|这是指向 Azure 存储帐户，其中应导出数据的共享的访问签名 (SA) URL。|

## <a name="response"></a>响应
如果成功，此方法返回 `202 Accepted` 响应代码。 它不返回任何响应正文中。 则响应中包含以下标头。

| 名称       | 说明 |
|:---------------|:----------|
| Location  | 若要检查请求的状态的 URL。 |
| 重试间隔后  | 以秒为单位的时间段。 请求 maker 应等待这长之后提交请求以检查的状态。 |


## <a name="example"></a>示例
##### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
##### <a name="response"></a>响应

```
{
  Location: https://graph.microsoft.com/beta/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
  Retry-After: 60
}
```

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: exportPersonalData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
