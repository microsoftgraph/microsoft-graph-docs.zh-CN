---
title: synchronization： secrets
description: 提供用于与目标系统建立连接的凭据。
ms.localizationpriority: medium
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: ab8c0b7925c65d814843fbdfd392b35b17f240f1
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62226297"
---
# <a name="synchronization-secrets"></a>synchronization： secrets

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供用于与目标系统建立连接的凭据。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     |Directory.ReadWrite.All  |
|委派（个人 Microsoft 帐户） |不支持。 |
|应用程序                            |Application.ReadWrite.OwnedBy、Directory.ReadWrite.All | 

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/secrets
```

## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|credentials|[synchronizationSecretKeyStringValuePair](../resources/synchronization-synchronizationsecretkeystringvaluepair.md) 集合|要验证的凭据。 当 **useSavedCredentials 参数为** 时忽略 `true` 。|

## <a name="response"></a>响应
如果密钥已成功保存，此方法将返回 响应 `204 No Content` 代码。 它不会在响应正文中返回任何内容。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "synchronization_secrets"
}-->
```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/secrets
Content-type: application/json

{
    "value": [
        {
            "key": "BaseAddress",
            "value": "user@domain.com"
        },
        {
            "key": "SecretToken",
            "value": "password-value"
        },
        {
            "key": "SyncNotificationSettings",
            "value": "{\"Enabled\":false,\"DeleteThresholdEnabled\":false}"
        },
        {
            "key": "SyncAll",
            "value": "false"
        }
    ]
}
```

### <a name="response"></a>响应
下面展示了示例响应。 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronization: secrets",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
