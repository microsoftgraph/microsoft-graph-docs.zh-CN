---
title: 列出更新类
description: 从 educationClasses 导航属性获取 educationClass 资源。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d2bb66f54155365e2db3f2cc8d4d8faf04eaf694
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232173"
---
# <a name="list-taughtclasses"></a>列出更新类

命名空间：microsoft.graph

获取 [educationUser](../resources/educationclass.md) 所拥有的 [educationClass 资源](../resources/educationuser.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | EduRoster.ReadBasic                         |
| 委派（个人 Microsoft 帐户） | 不支持                               |
| 应用程序                            | EduRoster.Read.All、EduRoster.ReadWrite.All |

> [!NOTE]
> 请注意，如果使用委派令牌，则用户只能看到有关其自己的类的信息。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/me/taughtClasses
GET /education/users/{educationUserId}/taughtClasses
```

## <a name="optional-query-parameters"></a>可选的查询参数

可以使用 OData 查询选项 `$orderby`，按 **displayName** 值对组织中的组进行排序，如下面的示例所示：

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

您还可以使用 和 `$filter` `$count` `$search` 查询参数来限制响应。

为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。 在添加或更新项目与在索引中可用之间可能会稍有延迟。

有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象的集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "list_educationclass"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/classes/{educationClassId}/members/{educationUserId}/taughtClasses
```

### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationClass)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationClass",
      "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
      "displayName": "String",
      "mailNickname": "String",
      "description": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "classCode": "String",
      "externalName": "String",
      "externalId": "String",
      "externalSource": "String",
      "externalSourceDetail": "String",
      "grade": "String",
      "term": {
        "@odata.type": "microsoft.graph.educationTerm"
      }
    }
  ]
}
```
