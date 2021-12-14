---
title: 列出团队
description: 列出组织中的所有团队
author: akhilkohlimicrosoft
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8c4a2d90f3c82c7066fee7c98aebbd3ba011c825
ms.sourcegitcommit: c99d3feb3ab5cae506c1f758bc277a637adc9111
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2021
ms.locfileid: "61432740"
---
# <a name="list-teams"></a>列出团队

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

列出组织中的所有[团队](../resources/team.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Team.ReadBasic.All，TeamSettings.Read.All，TeamSettings.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Team.ReadBasic.All，TeamSettings.Read.All，TeamSettings.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /teams
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持  `$filter`、`$select`、`$top`、`$skiptoken`、`$count` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。 |
| 接受  | application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回`200 OK`响应代码和[team](../resources/team.md)对象集合。

> [!Note]
> 目前，此 API 调用仅返回 [团队](../resources/team.md)的 **id**、**displayName** 和 **说明** 属性。 若要获取所有属性，请使用[获取团队](../api/team-get.md)操作。 

## <a name="examples"></a>示例

### <a name="example-1-get-a-list-of-teams"></a>示例 1：获取团队列表

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "get_teams"
}-->
```http
GET https://graph.microsoft.com/beta/teams
```
---

#### <a name="response"></a>响应
响应示例如下所示。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "172b0cce-e65d-44ce-9a49-91d9f2e8493a",
      "displayName": "Contoso Team",
      "description": "This is a Contoso team, used to showcase the range of properties supported by this API"
    },
    {
      "id": "890972b0cce-e65d-44ce-9a49-568hhsd7n",
      "displayName": "Contoso General Team",
      "description": "This is a general Contoso team"
    },
    ,
    {
      "id": "98678abcce0-e65d-44ce-9a49-9980bj8kl0e",
      "displayName": "Contoso API Team",
      "description": "This is Contoso API team"
    }
  ]
}
```

### <a name="example-2-use-filter-and-top-to-get-two-teams-with-a-display-name-that-starts-with-a"></a>示例 2：使用 $filter 和 $top 获取两个显示名称以"A"开头的团队

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "get_teams"
}-->

```http
GET https://graph.microsoft.com/beta/teams?$filter=startswith(displayName, 'A')&$top=2
```


#### <a name="response"></a>响应

响应示例如下所示。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "172b0cce-e65d-44ce-9a49-91d9f2e8493a",
      "displayName": "A Contoso Team",
      "description": "This is a Contoso team, used to showcase the range of properties supported by this API"
    },
    {
      "id": "890972b0cce-e65d-44ce-9a49-568hhsd7n",
      "displayName": "A Contoso Notification Team",
      "description": "This is a notification Contoso team"
    },
  ]
}
```

### <a name="example-3-use-filter-and-select-to-get-id-and-description-for-team-with-displayname-equals-a-contoso-team"></a>示例 3：使用 $filter 和 $select 获取 displayName 等于"A Contoso Team"的团队 ID 和说明

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "get_teams"
}-->
```http
GET https://graph.microsoft.com/beta/teams?$filter=displayName eq 'A Contoso Team'&$select=id,description
```
---

#### <a name="response"></a>响应
响应示例如下所示。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "172b0cce-e65d-44ce-9a49-91d9f2e8493a",
      "description": "This is a Contoso team, used to showcase the range of properties supported by this API"
    }
  ]
}
```


## <a name="see-also"></a>另请参阅
- [获取团队](../api/team-get.md)