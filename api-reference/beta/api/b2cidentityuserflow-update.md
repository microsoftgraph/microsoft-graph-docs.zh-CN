---
title: 更新 b2cIdentityUserFlow
description: 更新 b2cIdentityUserFlow 对象的属性。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bc030097cbfc6e57cbe841f6a0dd98660d1a12f7
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706229"
---
# <a name="update-b2cidentityuserflow"></a>更新 b2cIdentityUserFlow

命名空间：microsoft.graph

更新 [b2cIdentityUserFlow 对象](../resources/b2cidentityuserflow.md) 的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）|IdentityUserFlow.ReadWrite.All|
|委派（个人 Microsoft 帐户）| 不支持。|
|应用程序|IdentityUserFlow.ReadWrite.All|

工作或学校帐户需要属于以下角色之一：

* 全局管理员
* 外部标识用户流管理员

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象的 JSON 表示形式。

下表显示创建 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)后可以更新的属性。

|属性|类型|说明|
|:---|:---|:---|
|isLanguageCustomizationEnabled|布尔|该属性确定是否在 B2C 用户流中启用语言自定义。 默认情况下，不会为 B2C 用户流启用语言自定义。|
|defaultLanguageTag|字符串|指示在请求中未指定标记时所使用的 b2cIdentityUserFlow `ui_locale` 的默认语言。 此字段符合[RFC 5646。](https://tools.ietf.org/html/rfc5646)|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应 `200 OK` 代码和更新 [的 b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "update_b2cidentityuserflow"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp
Content-Type: application/json
Content-length: 469

{
  "isLanguageCustomizationEnabled": true,
  "defaultLanguageTag": "en",
}
```

### <a name="response"></a>响应

下面是一个响应示例。

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
}
-->

``` http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create b2CUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: update_b2cidentityuserflow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: update_b2cidentityuserflow/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
