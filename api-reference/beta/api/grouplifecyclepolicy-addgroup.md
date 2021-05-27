---
title: 'groupLifecyclePolicy: addGroup'
description: 将组添加到生命周期策略。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b35008f93cd4e7457ef83a2bc800423755157f59
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681163"
---
# <a name="grouplifecyclepolicy-addgroup"></a>groupLifecyclePolicy: addGroup

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将组添加到生命周期策略。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持 |
|应用程序 | Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a>请求标头

| 名称 | 说明 |
|:---------------|:----------|
| Authorization | Bearer {token}。必需。 |
| Content-Type  | application/json |

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数 | 类型 | 说明 |
|:---------------|:--------|:----------|
|groupId|Guid| 要添加到策略的组的 ID。 |

## <a name="response"></a>响应

如果成功，此方法返回 `200 OK` 响应代码。 如果组已添加到策略，便会在响应正文中返回 **true** 值。 否则，响应正文中返回 **false** 值。

## <a name="example"></a>示例

#### <a name="request"></a>请求

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}/addGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

#### <a name="response"></a>响应
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "value": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


