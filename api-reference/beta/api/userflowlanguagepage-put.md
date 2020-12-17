---
title: 更新 userFlowLanguagePage
description: 更新 userFlowLanguagePage 对象中的值。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4e73897facf0407bed489a93c057c0c7f78436d5
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706302"
---
# <a name="update-userflowlanguagepage"></a>更新 userFlowLanguagePage

命名空间：microsoft.graph

更新 userFlowLanguagePage 对象中的值。 只能更新 overridesPage 中的值，overridesPage 用于在用户流定义的用户旅程中自定义向用户显示的值。

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

若要引用对象中的内容，必须使用 `$value` 。 这将返回对象中的内容，并允许你直接引用它。

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2cUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
PUT /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [userFlowLanguagePage](../resources/userflowlanguagepage.md)中包含的值的 JSON 表示形式。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "update_overridespages"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en/overridesPages/phonefactor/$value
Content-Type: application/json

{
  "LocalizedStrings": [
        {
            "ElementType": "UxElement",
            "ElementId": null,
            "StringId": "alert_message",
            "Override": true,
            "Value": "Are you sure that you want to cancel your selection?"
        }
    ]
}
```

### <a name="response"></a>响应

下面是一个响应示例。

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
