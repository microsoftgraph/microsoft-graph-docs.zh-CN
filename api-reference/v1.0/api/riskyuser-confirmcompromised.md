---
title: riskyUser：confirmComprom一
description: 确认用户受到威胁
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3bd85442ded90d07fea8ea3a558bf738ced5c2c5
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60939089"
---
# <a name="riskyuser-confirmcompromised"></a>riskyUser：confirmComprom一
命名空间：microsoft.graph

>**注意：** riskyUsers API 需要一个Azure AD Premium P2许可证。

确认一个或多个 [riskyUser](../resources/riskyuser.md) 对象受到威胁。 此操作将目标用户的风险级别设置得较高。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | IdentityRiskyUser.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | IdentityRiskyUser.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityProtection/riskyUsers/confirmCompromised
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|Description|
|:---|:---|:---|
|userIds|String 集合|在请求正文中指定要消除的风险用户 ID。|



## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "riskyuser_confirmcompromised"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised
Content-Type: application/json

{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
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


