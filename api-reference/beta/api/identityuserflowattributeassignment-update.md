---
title: 更新 identityUserFlowAttributeAssignment
description: 更新 userAttributeAssignments 对象的属性。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2b9b5e39cd8d7462b678608ae74727eacdf101cb
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581326"
---
# <a name="update-identityuserflowattributeassignment"></a>更新 identityUserFlowAttributeAssignment

命名空间：microsoft.graph

更新 identityUserFlowAttributeAssignment 对象的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|IdentityUserFlow|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|IdentityUserFlow|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
PATCH /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象的 JSON 表示形式。

下表显示了可在 [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)中更新的属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|用户流中的 identityUserFlowAttribute 的显示名称。|
|isOptional|布尔值|确定 identityUserFlowAttribute 是否为可选。 `true` 表示用户不必提供值。 `false` 表示用户不能完成注册，而无需提供值。|
|requiresVerification|布尔值|确定 identityUserFlowAttribute 是否需要验证。 这仅用于验证用户的电话号码或电子邮件地址。|
|userAttributeValues|[userAttributeValuesItem](../resources/userattributevaluesitem.md) 集合|用户流属性的输入选项。 仅当 userInputType 为、或时才适用 `radioSingleSelect` `dropdownSingleSelect` `checkboxMultiSelect` 。|
|userInputType|identityUserFlowAttributeInputType|用户流属性的输入类型。 可取值为：`textBox`、`dateTimeDropdown`、`radioSingleSelect`、`dropdownSingleSelect`、`emailBox`、`checkboxMultiSelect`。|

## <a name="response"></a>响应

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "update_userattributeassignments"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/{id}
Content-Type: application/json

{
  "userInputType": "textBox"
}
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
