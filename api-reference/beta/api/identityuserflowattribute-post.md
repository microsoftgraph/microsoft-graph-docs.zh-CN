---
title: 创建 identityUserFlowAttribute
description: 创建新的 identityUserFlowAttribute 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 443ac0848e7ace309172dc0ca38d9a191acb9635
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742362"
---
# <a name="create-identityuserflowattribute"></a>创建 identityUserFlowAttribute

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [identityUserFlowAttribute](../resources/identityuserflowattribute.md) 对象。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）|IdentityUserFlow|
|委派（个人 Microsoft 帐户）| 不支持。|
|应用程序|IdentityUserFlow|

工作或学校帐户需要属于下列角色之一：

* 全局管理员
* 外部标识用户流属性管理员

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlowAttributes
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---------------|:----------|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)的 JSON 表示形式。

|属性|类型|说明|
|:---------------|:--------|:----------|
|id|String|用户流属性的标识符。 这是一个自动创建的只读属性。|
|displayName|String|用户流属性的显示名称。|
|说明|String|用户流属性的说明。 在注册时，会向用户显示。|
|userFlowAttributeType|String|用户流属性的类型。 这是一个自动设置的只读属性。 根据属性的类型，此属性的值将为 `builtIn` 或 `custom` 。|
|DataType|String|用户流属性的数据类型。 一旦创建了自定义用户流属性，就不能修改此属性。 **数据类型**的受支持的值为：<br/><ul><li>`string` ：表示 identityUserFlowAttribute 的数据类型为字符串。 </li><li>`boolean` ：表示 identityUserFlowAttribute 的数据类型是一个布尔值。</li><li>`int64` ：表示 identityUserFlowAttribute 的数据类型为整数。</li></ul>|

## <a name="response"></a>响应

如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [identityUserFlowAttribute](../resources/identityuserflowattribute.md) 对象。 如果失败，将返回 `4xx` 错误并显示具体详细信息。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "create_userFlowAttribute_from_userFlowAttributes"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/userFlowAttributes
Content-type: application/json

{
  "displayName": "Hobby",
  "description": "Your hobby",
  "dataType": "string",
}
```

### <a name="response"></a>响应

下面展示了示例响应。

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/userFlowAttributes/extension_7a95ecd9489b4fb9a45722b913c4703b_Hobby
Content-type: application/json

{
    "id": "extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby",
    "displayName": "Hobby",
    "description": "Your hobby",
    "userFlowAttributeType": "custom",
    "dataType": "string"
}
```
