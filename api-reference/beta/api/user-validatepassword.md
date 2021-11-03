---
title: user： validatePassword
description: 针对组织的密码验证策略检查用户的密码，并报告密码是否有效。
author: yyuank
ms.localizationpriority: medium
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 46eb935f2ad6d932f61cdfb8552a306bfc498682
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697245"
---
# <a name="user-validatepassword"></a>user： validatePassword
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

针对组织的密码验证策略检查用户的密码，并报告密码是否有效。 使用此操作在用户输入密码时提供有关密码强度实时反馈。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）| User.ReadWrite、User.ReadWrite.All |
|委派（个人 Microsoft 帐户）| 不支持。 |
|应用程序| 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/validatePassword
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了此操作所需的参数。

|参数|类型|说明|
|:---|:---|:---|
|密码|String| 此操作要验证的密码。|

## <a name="response"></a>响应

如果成功，此操作在响应正文中返回 响应代码和 `200 OK` [passwordValidationInformation](../resources/passwordvalidationinformation.md) 对象。

## <a name="examples"></a>示例 

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "user_validatepassword"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/validatePassword
Content-Type: application/json

{
    "password": "1234567890"
}
```


### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordValidationInformation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
    "isValid": false,
    "validationResults": [
        {
            "ruleName": "password_not_meet_complexity",
            "validationPassed": false,
            "message": "Password does not meet complexity requirements."
        }
    ]
}
```

