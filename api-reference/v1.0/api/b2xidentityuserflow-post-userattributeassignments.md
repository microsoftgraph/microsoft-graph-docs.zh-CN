---
title: 创建 userAttributeAssignments
description: 在 b2xIdentityUserFlow 中创建新的 identityUserFlowAttributeAssignment 对象。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8daa8a13baa6e08ebfdc666d2f783fbacb82645a
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882919"
---
# <a name="create-userattributeassignments"></a>创建 userAttributeAssignments

命名空间：microsoft.graph

在 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)中创建新的 identityUserFlowAttributeAssignment 对象。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|IdentityUserFlow.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|IdentityUserFlow.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2xUserFlows/{id}/userAttributeAssignments
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象的 JSON 表示形式。

下表显示创建 [identityUserFlowAttributeAssignment 时所需的属性](../resources/identityuserflowattributeassignment.md)。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|用户显示名称中的 identityUserFlowAttribute 的组。|
|isOptional|Boolean|确定 identityUserFlowAttribute 是否可选。 `true` 表示用户不必提供值。 `false` 表示用户无法在未提供值的情况下完成注册。|
|requiresVerification|Boolean|确定 identityUserFlowAttribute 是否需要验证。 这仅用于验证用户的电话号码或电子邮件地址。|
|userAttributeValues|[userAttributeValuesItem](../resources/userattributevaluesitem.md) 集合|用户流属性的输入选项。 仅在 userInputType 为 `radioSingleSelect` 、 `dropdownSingleSelect` 或 时适用 `checkboxMultiSelect` 。|
|userInputType|identityUserFlowAttributeInputType|用户流属性的输入类型。 可取值为：`textBox`、`dateTimeDropdown`、`radioSingleSelect`、`dropdownSingleSelect`、`emailBox`、`checkboxMultiSelect`。|
|userAttribute|[identityUserFlowAttribute](../resources/identityuserflowattribute.md)|要包括在用户流分配中的用户流属性的标识符。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_identityuserflowattributeassignment_from__2"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments
Content-Type: application/json

{
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "Shoe size",
    "userAttributeValues": [],
    "userAttribute": {
        "id": "extension_guid_shoeSize"
    }
}
```

### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment"
}
-->

``` http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/extension_guid_shoeSize
Content-Type: application/json

{
    "id": "extension_guid_shoeSize",
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "Shoe size",
    "userAttributeValues": []
}
```
