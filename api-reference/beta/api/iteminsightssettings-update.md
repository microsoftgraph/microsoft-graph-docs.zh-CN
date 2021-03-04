---
title: 更新 itemInsights
description: 更新 itemInsightsSettings 对象的属性
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: bf7a661663779b618d1de191386294cdab5b915f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443816"
---
# <a name="update-iteminsightssettings"></a>更新 itemInsightsSettings

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新指定 [itemInsightsSettings 资源](../resources/iteminsightssettings.md) 的属性。

若要了解如何为组织自定义项目见解隐私，请参阅 [自定义见解隐私](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0)。 

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|Application | 不支持。 |

>**注意：** 对此操作使用委派权限要求登录用户拥有全局管理员角色。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{organizationId}/settings/itemInsights
```

## <a name="request-headers"></a>请求标头

| 标头       | 值|
|:-----------|:------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|isEnabledInOrganization|布尔| `true` 如果启用了组织项目见解; `false` 如果为所有用户禁用组织项目见解，则无例外。 默认值为 `true`。 可选。|
|disabledForGroup|String| 已禁用成员的项见解的 Azure AD 组的 ID。 默认值为 `empty`。 可选。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码和 `200 OK` [itemInsightsSettings](../resources/iteminsightssettings.md) 对象。

>**注意：** 此操作验证指定 **itemInsightsSettings** 资源的属性值的有效性。 如果 **已设置 disabledForGroup** 属性，此操作不会检查相应的 Azure AD 组是否存在。 这意味着，如果将 **disabledForGroup** 设置为不存在或之后已删除的 Azure AD 组，则此操作将无法识别任何组成员身份，并禁用对特定用户的项目见解。 如果 **isEnabledInOrganization** 设置为 ，则此操作将为组织中所有用户 `true` 启用见解。 

## <a name="example"></a>示例 

### <a name="request"></a>请求

下面是管理员如何更新 **"disabledForGroup"** 隐私设置以禁止显示特定 Azure AD 组的用户项目见解的示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_iteminsightssettings"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
Content-type: application/json

{
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-iteminsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-iteminsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-iteminsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-iteminsightssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应

下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemInsightsSettings",
  "name": "update_iteminsightssettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```


