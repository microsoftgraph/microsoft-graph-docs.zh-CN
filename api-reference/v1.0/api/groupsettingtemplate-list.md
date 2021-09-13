---
title: List groupSettingTemplates
description: 检索可用的 groupSettingTemplates 对象的列表。
author: Jordanndahl
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5b1417f9b2b85252aa8a250580e46c252b178f53
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022280"
---
# <a name="list-groupsettingtemplates"></a>List groupSettingTemplates

命名空间：microsoft.graph

组设置模板表示一组模板，用于创建组设置并在租户内使用。此操作将检索可用 groupSettingTemplates 对象的列表。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Directory.Read.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$select` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

> **注意：** 不支持 $filter。

## <a name="request-headers"></a>请求标头
| 名称 | 说明 |
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupSettingTemplate](../resources/groupsettingtemplate.md) 对象集合。

## <a name="example"></a>示例
##### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplates"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettingTemplates
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettingtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettingtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettingtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettingtemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应

注意：为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates",
  "value": [
    {
      "id": "08d542b9-071f-4e16-94b0-74abb372e3d9",
      "deletedDateTime": null,
      "displayName": "Group.Unified.Guest",
      "description": "Settings for a specific Unified Group",
      "values": [
        {
          "name": "AllowToAddGuests",
          "type": "System.Boolean",
          "defaultValue": "true",
          "description": "Flag indicating if guests are allowed in a specific Unified Group."
        }
      ]
    },
    {
      "id": "80661d51-be2f-4d46-9713-98a2fcaec5bc",
      "deletedDateTime": null,
      "displayName": "Prohibited Names Settings",
      "description": "Setting templates define the different settings that can be used for the associated ObjectSettings. This template defines settings that can be used for managing tenant-wide prohibited names settings.",
      "values": [
        {
          "name": "CustomBlockedSubStringsList",
          "type": "System.String",
          "defaultValue": "",
          "description": "A comma delimited list of substring reserved words to block for application display names."
        },
        {
          "name": "CustomBlockedWholeWordsList",
          "type": "System.String",
          "defaultValue": "",
          "description": "A comma delimited list of reserved words to block for application display names."
        }
      ]
    }  
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
