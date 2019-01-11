---
title: 注册 governanceResource
description: 在 PIM 中注册一个非托管的 governanceResource 对象。
localization_priority: Normal
ms.openlocfilehash: ce439d53eb9f017340f561ca509e8da43dbafbfc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837749"
---
# <a name="register-governanceresource"></a>注册 governanceResource

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

在特权身份管理中注册一个非托管的[governanceResource](../resources/governanceresource.md)对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

>**注意：** 此 API 还需要请求者对资源具有至少一个活动角色分配。

|权限类型      | Permissions              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureResources  |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | PrivilegedAccess.ReadWrite.AzureResources |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a>可选的查询参数
此方法**仅**支持`$select`和`$expand` [OData 查询参数](/graph/query-parameters)，以帮助自定义的响应。

### <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | 持有者 {code}|
| Content-type  | application/json|

### <a name="request-body"></a>请求正文

|参数      |类型                 |是否必需 |说明|
|:-------------|:----------------------|:--------|:----------|
|externalId    |String                 |✓        |要在 PIM 中注册的资源 externalId。|

### <a name="response"></a>响应
如果成功，此方法返回`200 OK`响应。

### <a name="example"></a>示例
本示例演示如何注册的 Azure 订阅 Wingtip Toys-prod 移。
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a>请求
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
