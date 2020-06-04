---
title: 更新 authenticationFlowsPolicy
description: 更新 authenticationFlowsPolicy 对象的布尔 selfServiceSignUp 属性。
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 626e1dc8a851f2c8da6a9bb815a4e783cf44e7d2
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556384"
---
# <a name="update-authenticationflowspolicy"></a>更新 authenticationFlowsPolicy

命名空间：microsoft.graph

更新[authenticationFlowsPolicy](../resources/authenticationflowspolicy.md)对象的布尔**selfServiceSignUp**属性。 无法修改属性**id**、**类型**和**说明**。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|AuthenticationFlows|
|委派（个人 Microsoft 帐户）|不支持|
|Application|AuthenticationFlows|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，可以提供[authenticationFlowsPolicy](../resources/authenticationflowspolicy.md)对象的 JSON 表示形式（但不是必需的）。

下表显示了在更新[authenticationFlowsPolicy](../resources/authenticationflowspolicy.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|selfServiceSignUp|[selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md)|自助注册配置。|

## <a name="response"></a>响应

如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。

## <a name="example"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "update_authenticationflowspolicy"
}
-->
```http
PATCH https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
Content-Type: application/json

{
  "selfServiceSignUp": {
    "isEnabled": true
  }
}
```

### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
} -->
``` http
HTTP/1.1 204 No Content
```
