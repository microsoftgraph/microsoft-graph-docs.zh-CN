---
title: 获取 itemInsights
description: 检索 itemInsightsSettings 对象的属性
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: aae37d83bafb9c8ad59dcbce1de6b8875ee091dd
ms.sourcegitcommit: 70e09ebbf67f49a0c64ab7a275e751f8a68b8696
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/27/2020
ms.locfileid: "48771790"
---
# <a name="get-iteminsightssettings"></a>获取 itemInsightsSettings

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [itemInsightsSettings](../resources/iteminsightssettings.md) 对象的属性。

若要了解如何为你的组织自定义项目见解隐私，请参阅 [自定义见解隐私](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0)。 

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.Read、User.ReadWrite |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |

>**注意：** 对此操作使用委派权限时，需要已登录用户拥有全局管理员角色。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->

```http
GET /organization/{organizationId}/settings/itemInsights
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:----------|
| Authorization  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [itemInsightsSettings](../resources/iteminsightssettings.md) 对象。

>**注意：** 此操作将验证指定的 **itemInsightsSettings** 资源的属性值的有效性。 如果设置了 **disabledForGroup** 属性，则此操作不检查是否存在相应的 Azure AD 组。 这意味着，如果您将 **disabledForGroup** 设置为不存在或随后删除的 Azure AD 组，则此操作将无法识别任何组成员身份并为任何特定用户禁用项目见解。 如果将 **isEnabledInOrganization** 设置为 `true` ，该操作将为组织中的所有用户启用见解。 

## <a name="example"></a>示例

##### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_iteminsightssettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-iteminsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-iteminsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-iteminsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应

下面是一个响应示例。 
> **注意：** 为简洁起见，可能会截断此处展示的响应对象。 将从实际调用中返回所有属性。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemInsightsSettings",
  "name": "get_iteminsightssettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```


