---
title: 更新见解
description: 更新 insightsSettings 对象的属性
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 7af541c033cebb9409ac1bf61a8470b1c67726a0
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322758"
---
# <a name="update-insightssettings"></a>更新 insightsSettings

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新隐私设置以显示或返回组织中指定的见解类型。 设置类型可以是项目见解或人员见解。

若要了解有关为组织自定义见解隐私的信息，请参阅：
-  [自定义项目见解隐私](/graph/insights-customize-item-insights-privacy) 
-  [自定义人员见解隐私](/graph/insights-customize-people-insights-privacy)

## <a name="permissions"></a>权限

若要调用此 API，需要以下权限之一。 若要了解更多信息，包括如何选择权限，请参阅 [权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |


>**注意：** 对此操作使用委派权限要求登录用户拥有全局管理员角色。
## <a name="http-request"></a>HTTP 请求

若要更新项目见解的设置：：
<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{organizationId}/settings/itemInsights
```

若要更新人员见解设置：
<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{organizationId}/settings/peopleInsights
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
|isEnabledInOrganization|布尔值| `true` 如果为组织启用了指定类型的见解;如果为所有用户禁用了指定类型的见解，则 `false` 无例外。 默认值为“`true`”。 可选。|
|disabledForGroup|String| 组 id，Azure AD组的成员禁用其指定类型的见解。 默认值为“`empty`”。 可选。|

>**注意：** 如果将 **disabledForGroup** 属性值包括在请求正文中，则此操作不会验证该值。 如果将 **disabledForGroup** 属性设置为字符串，则此操作不会检查是否存在相应的Azure AD组。 这意味着，如果将 **disabledForGroup** 设置为不存在或随后被删除的 Azure AD 组，则此操作将无法识别任何组成员身份，并禁用对特定用户的项或人员见解。 如果 **isEnabledInOrganization** 设置为 ，则操作将为组织中所有用户启用指定 `true` 类型的见解。  
## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [insightsSettings](../resources/insightssettings.md) 对象。

## <a name="examples"></a>示例 

### <a name="example-1-update-settings-for-item-insights"></a>示例 1：更新项目见解的设置
#### <a name="request"></a>请求

下面是一个示例请求，显示管理员如何更新 **"disabledForGroup"** 隐私设置，以禁止显示特定用户组中用户Azure AD见解。


<!-- {
  "blockType": "request",
  "name": "update_insightssettings_iteminsightrequest"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
Content-type: application/json

{
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```


#### <a name="response"></a>响应

下面是一个响应示例。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.insightsSettings",
  "name": "update_insightssettings_iteminsightrequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```


### <a name="example-2-update-settings-for-people-insights"></a>示例 2：更新人员见解设置
#### <a name="request"></a>请求

下面是一个请求示例，显示管理员如何更新 **"disabledForGroup"** 隐私设置，以禁止显示特定用户组中用户Azure AD见解。


<!-- {
  "blockType": "request",
  "name": "update_insightssettings_peopleinsightsrequest"
}-->
```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/peopleInsights
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```



### <a name="response"></a>响应

下面展示了示例响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.insightsSettings",
  "name": "update_insightssettings_peopleinsightsrequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```


 107 api-reference/beta/api/iteminsightssettings-get.md 
