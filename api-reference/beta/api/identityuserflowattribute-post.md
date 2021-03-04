---
title: 创建 identityUserFlowAttribute
description: 创建新的 identityUserFlowAttribute 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: f6cdbf3d22e7b51e656e3dbe3d44180232a1467b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435252"
---
# <a name="create-identityuserflowattribute"></a>创建 identityUserFlowAttribute

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [identityUserFlowAttribute](../resources/identityuserflowattribute.md) 对象。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）|IdentityUserFlow.ReadWrite.All|
|委派（个人 Microsoft 帐户）| 不支持。|
|Application|IdentityUserFlow.ReadWrite.All|

工作或学校帐户需要属于以下角色之一：

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
|id|String|用户流属性的标识符。 这是自动创建的只读属性。|
|displayName|String|用户显示名称属性的属性值。|
|说明|String|用户流属性的说明。 它在注册时显示给用户。|
|userFlowAttributeType|String|用户流属性的类型。 这是自动设置的只读属性。 根据属性的类型，此属性的值将为 `builtIn` 或 `custom` 。|
|DataType|String|用户数据类型属性的属性值。 创建自定义用户流属性后，无法修改此属性。 dataType **支持的值** 包括：<br/><ul><li>`string` ： 表示 identityUserFlowAttribute 的 dataType 是字符串。 </li><li>`boolean` ： 表示 identityUserFlowAttribute 的 dataType 为布尔值。</li><li>`int64` ： 表示 identityUserFlowAttribute 的 dataType 是一个整数。</li></ul>|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码和 `201 Created` [identityUserFlowAttribute](../resources/identityuserflowattribute.md) 对象。 如果失败，将返回 `4xx` 错误并显示具体详细信息。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-userflowattribute-from-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-userflowattribute-from-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-userflowattribute-from-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-userflowattribute-from-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
