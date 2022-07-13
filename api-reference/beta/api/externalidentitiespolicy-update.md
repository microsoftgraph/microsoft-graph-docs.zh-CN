---
title: 更新 externalIdentitiesPolicy
description: 更新租户范围的 externalIdentitiesPolicy 对象的设置，该对象控制外部用户是否可以通过自助服务控件离开 Azure AD 租户。
author: KuiGithui
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 918bc089306c51d28a4afb61fc4a4038bb8eb049
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768353"
---
# <a name="update-externalidentitiespolicy"></a>更新 externalIdentitiesPolicy
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新租户范围的 [externalIdentitiesPolicy](../resources/externalidentitiespolicy.md) 对象的设置，该对象控制外部用户是否可以通过自助服务控件离开 Azure AD 租户。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Policy.ReadWrite.ExternalIdentities|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|Policy.ReadWrite.ExternalIdentities|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/externalIdentitiesPolicy
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

|属性|类型|说明|
|:---|:---|:---|
|allowDeletedIdentitiesDataRemoval|Boolean|通知 Azure AD 在用户在其主租户中删除用户时，是否从来宾租户中清理有关外部标识的用户信息。 必需。|
|allowExternalIdentitiesToLeave|Boolean|通知 Azure AD 在用户在其主租户中删除用户时，是否从来宾租户中清理有关外部标识的用户信息。 必需。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "update_externalidentitiespolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/externalIdentitiesPolicy

{
  "allowExternalIdentitiesToLeave":false
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

