---
title: 获取 adminConsentRequestPolicy
description: 读取 adminConsentRequestPolicy 对象的属性和关系。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f9a6d19c1671265034ca5f2663ab55aa701eeda8
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469539"
---
# <a name="get-adminconsentrequestpolicy"></a>获取 adminConsentRequestPolicy

命名空间：microsoft.graph

读取 [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) 对象的属性和关系。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Policy.Read.All、Policy.ReadWrite.ConsentRequest、Directory.Read.All、Directory.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|Policy.Read.All、Policy.ReadWrite.ConsentRequest、Directory.Read.All、Directory.ReadWrite.All|

代表用户进行呼叫时，用户需要属于以下目录角色之一。 若要了解有关目录角色的信息，请参阅 [Azure AD 内置角色](/azure/active-directory/roles/permissions-reference)：
+ 全局管理员
+ 全局读取者
+ 云 应用程序管理员
+  应用程序管理员

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/adminConsentRequestPolicy
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持  `$select`   OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get_adminconsentrequestpolicy"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/policies/adminConsentRequestPolicy
```

### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.adminConsentRequestPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/adminConsentRequestPolicy/$entity",
  "isEnabled": true,
  "notifyReviewers": false,
  "remindersEnabled": false,
  "requestDurationInDays": 0,
  "version": 0,
  "reviewers": [
    {
      "query": "/users/906e0ee5-6372-4cc8-8248-fdf2846b48ed",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    },
    {
      "query": "/users/daddef1a-acb0-4f62-96d0-49df2495d657",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ]
}
```
