---
title: 更新 trustFrameworkPolicy
description: '此操作将更新现有的 trustFrameworkPolicy 对象，如果不存在，则创建一个。 '
ms.localizationpriority: medium
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0a944c9296ad414064a8fe002d75301f3ecb8875
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730282"
---
# <a name="update-or-create-trustframeworkpolicy"></a>更新或创建 trustFrameworkPolicy

命名空间：microsoft.graph

>**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

更新现有的 [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) 或创建一个（如果不存在）。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）|Policy.ReadWrite.TrustFramework|
|委派（个人 Microsoft 帐户）| 不支持。|
|应用程序|Policy.ReadWrite.TrustFramework|

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

在请求正文中，提供 [trustFrameworkPolicy 对象的](../resources/trustframeworkpolicy.md) XML 表示形式。 

>**注意：** 内容类型必须为 `application/xml` 。

## <a name="response"></a>响应

响应将为以下操作之一：
- 如果存在 [trustFrameworkPolicy，](../resources/trustframeworkpolicy.md) 则成功的请求将返回 响应 `200 OK` 代码。
- 如果 [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) 不存在，则成功的请求将返回 `201 Created` 响应代码。
- 如果失败，将返回 `4xx` 错误并显示具体详细信息。

## <a name="example"></a>示例

以下示例更新 **trustFrameworkPolicy**。

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


