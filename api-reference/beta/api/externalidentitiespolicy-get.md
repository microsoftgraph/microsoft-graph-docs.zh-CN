---
title: 获取 externalIdentitiesPolicy
description: 读取租户范围 externalIdentitiesPolicy 对象的属性和关系，该对象控制外部用户是否可以通过自助服务控件离开 Azure AD 租户。
author: KuiGithui
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: dd7defc8cdbedf1d4d47120edd791bdda4fb829f
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768341"
---
# <a name="get-externalidentitiespolicy"></a>获取 externalIdentitiesPolicy
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取租户范围 [externalIdentitiesPolicy](../resources/externalidentitiespolicy.md) 对象的属性和关系，该对象控制外部用户是否可以通过自助服务控件离开 Azure AD 租户。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Policy.Read.All、Policy.ReadWrite.ExternalIdentities|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|Policy.Read.All、Policy.ReadWrite.ExternalIdentities|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/externalIdentitiesPolicy
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法不支持帮助自定义响应的 OData 查询参数。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [externalIdentitiesPolicy](../resources/externalidentitiespolicy.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_externalidentitiespolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/externalIdentitiesPolicy
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalIdentitiesPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/externalIdentitiesPolicy/$entity",
    "id": "externalIdentityPolicy",
    "deletedDateTime": null,
    "allowExternalIdentitiesToLeave": true,
    "allowDeletedIdentitiesDataRemoval": false,
    "displayName": "External Identities Policy"
  }
}
```

