---
title: 更新 itemInsights
description: 更新 itemInsightsSettings 对象的属性
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: de19cf6f33ed0c5b1930077232945564115cd14a
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435003"
---
# <a name="update-iteminsightssettings"></a>更新 itemInsightsSettings

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新指定的[itemInsightsSettings](../resources/iteminsightssettings.md)资源的属性。

若要了解如何为你的组织自定义项目见解隐私，请参阅[自定义见解隐私](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0)。 

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.ReadWrite |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | User.ReadWrite |

>**注意：** 对此操作使用委派权限时，需要已登录用户拥有全局管理员角色。

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
|isEnabledInOrganization|布尔| `true`如果启用了组织项目见解，则为`false`如果对不例外的所有用户禁用了组织项目见解。 默认值为 `true`。 可选。|
|disabledForGroup|字符串| Azure AD 组的 ID，其中成员的项目见解已禁用。 默认值为 `empty`。 可选。|

## <a name="response"></a>响应

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[itemInsightsSettings](../resources/iteminsightssettings.md)对象。

>**注意：** 此操作将验证指定的**itemInsightsSettings**资源的属性值的有效性。 如果设置了**disabledForGroup**属性，则此操作不检查是否存在相应的 Azure AD 组。 这意味着，如果您将**disabledForGroup**设置为不存在或随后删除的 Azure AD 组，则此操作将无法识别任何组成员身份并为任何特定用户禁用项目见解。 如果将**isEnabledInOrganization**设置为 `true` ，该操作将为组织中的所有用户启用见解。 

## <a name="example"></a>示例 

### <a name="request"></a>请求

以下是有关管理员更新 "**disabledForGroup**" 隐私设置以禁止显示用户的特定 Azure AD 组的项目见解的示例请求。
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
