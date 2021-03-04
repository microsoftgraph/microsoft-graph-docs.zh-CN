---
title: governanceResource：register
description: 在 PIM 中注册 governanceResource 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: fed82587a1132b6c39e6e27e09546906792486b0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435941"
---
# <a name="governanceresource-register"></a>governanceResource：register

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Privileged Identity Management 中注册 [governanceResource](../resources/governanceresource.md) 对象。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。

>**注意：** 此 API 还要求请求者至少对资源角色分配一个活动应用程序。

### <a name="azure-resources"></a>Azure 资源

| 权限类型 | 权限 |
|:--------------- |:----------- |
| 委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureResources |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application | 不支持。 |

### <a name="azure-ad"></a>Azure AD

| 权限类型 | 权限 |
|:--------------- |:----------- |
| 委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureAD |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application | 不支持。 |

### <a name="groups"></a>组

|权限类型 | 权限 |
|:-------------- |:----------- |
| 委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureADGroups |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法 **仅** 支持和 `$select` `$expand` [OData](/graph/query-parameters) 查询参数来帮助自定义响应。

## <a name="request-headers"></a>请求标头

| 名称 | 说明 |
|:---- |:----------- |
| Authorization | 持有者 {token} |
| Content-type | application/json |

## <a name="request-body"></a>请求正文

| 属性 | 类型 | 说明 |
|:---------- |:---- |:----------- |
| externalId | String | 在 PIM 中注册的资源的外部标识符。 如果注册订阅，标识符是预先预置的订阅标识符 `/subscriptions/` 。 例如，`/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`。 |

## <a name="response"></a>响应

如果成功，此方法将返回 `200 OK` 响应。

## <a name="example"></a>示例

以下示例演示如何调用此 API。
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a>请求
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a>响应
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
<!--
{
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


