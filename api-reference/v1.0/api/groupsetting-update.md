---
title: 更新 groupSetting
description: 更新特定组设置对象的属性。
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 604e4275f1b5d49fab3d866b6845d820f67cd0ec
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211275"
---
# <a name="update-groupsetting"></a>更新 groupSetting

命名空间：microsoft.graph

为租户范围的组设置或特定的[组](../resources/group.md)设置更新 [groupSetting](../resources/groupsetting.md) 对象的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | Directory.ReadWrite.All                     |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| Application                            | Directory.ReadWrite.All                     |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

更新租户范围的设置。

```http
PATCH /groupSettings/{groupSettingId}
```

<!-- { "blockType": "ignored" } -->

更新特定于组的设置。

```http
PATCH /groups/{groupId}/settings/{groupSettingId}
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明        |
| :------------ | :----------------- |
| Authorization | {token}。 必填。 |
| Content-Type  | application/json   |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。

| 属性 | 类型                                                    | 说明                                                                                                      |
| :------- | :------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------- |
| 值   | [settingValue](../resources/settingvalue.md) 集合 | 更新后的值集。 必须包括整个集合集。 不能更新一组值。 |

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="example-1-update-a-tenant-wide-group-setting"></a>示例 1：更新租户范围的组设置

在此示例中， `84af2ca5-c274-41bf-86e4-6e374ec4def6` 是租户范围 **groupSetting** 对象的标识符。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_tenant_groupsetting"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/groupSettings/84af2ca5-c274-41bf-86e4-6e374ec4def6
Content-type: application/json

{
    "values": [
        {
            "name": "AllowToAddGuests",
            "value": "false"
        }
    ]
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tenant-groupsetting-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tenant-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tenant-groupsetting-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tenant-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tenant-groupsetting-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/update-tenant-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tenant-groupsetting-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/update-tenant-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-tenant-groupsetting-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/update-tenant-groupsetting-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-group-setting"></a>示例 2：更新特定组设置

在此示例中， `0167b5af-f3d1-4910-82d2-398747fa381c` 是组的标识符，并且 `fa6df613-159b-4f94-add2-7093f961900b` 是 groupSetting 对象的标识符。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/groups/0167b5af-f3d1-4910-82d2-398747fa381c/settings/fa6df613-159b-4f94-add2-7093f961900b
Content-type: application/json

{
  "values": [
    {
      "name": "AllowToAddGuests",
      "value": "true"
    }
  ]
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-groupsetting-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/update-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-groupsetting-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/update-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-groupsetting-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/update-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-groupsetting-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/update-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-groupsetting-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/update-groupsetting-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
