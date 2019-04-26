---
title: 更新 trustFrameworkPolicy
description: '此操作将更新现有的 trustFrameworkPolicy 对象, 如果不存在, 则创建一个。 '
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1cb40c5a70056990bfa7d00443289bbcd565707d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335085"
---
# <a name="update-or-create-trustframeworkpolicy"></a>更新或创建 trustFrameworkPolicy

>**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

更新现有[trustFrameworkPolicy](../resources/trustframeworkpolicy.md) , 如果不存在, 则创建一个。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）|TrustFramework、全部写读。|
|委派（个人 Microsoft 帐户）| 不支持。|
|应用程序|不支持。|

工作或学校帐户必须是租户的全局管理员。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PUT /trustFramework/policies/{id}/$value
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---------------|:----------|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/xml。 必需。|

## <a name="request-body"></a>请求正文

在请求正文中, 提供[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)对象的 XML 表示形式。 

>**注意:** 内容类型必须为`application/xml`。

## <a name="response"></a>响应

响应将为以下之一:
- 如果存在[trustFrameworkPolicy](../resources/trustframeworkpolicy.md) , 则成功的请求将返回`200 OK`响应代码。
- 如果[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)不存在, 则成功的请求将返回`201 Created`响应代码。
- 如果失败，将返回 `4xx` 错误并显示具体详细信息。

## <a name="example"></a>示例

下面的示例更新**trustFrameworkPolicy**。

##### <a name="request"></a>请求

<!-- {
  "blockType": "ignored",
  "name": "update_trustframeworkpolicy"
}-->
```http
PUT https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base/$value
Content-Type: application/xml

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```

##### <a name="response"></a>响应

<!-- {
  "blockType": "ignored",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/xml

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_Test" PublicPolicyUri="http://tenantName.onmicrosoft.com/B2C_1A_Test">
    .....
    ....
    <!---PolicyContent-->
    ....
    ....
</TrustFrameworkPolicy>
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update trustframeworkpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
