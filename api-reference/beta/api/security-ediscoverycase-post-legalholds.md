---
title: 创建 ediscoveryHoldPolicy
description: 创建新的 ediscoveryHoldPolicy 对象。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: ad795f9bc03b6cc131b4b2ae57442b06a1447eee
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442546"
---
# <a name="create-ediscoveryholdpolicy"></a>创建 ediscoveryHoldPolicy
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|eDiscovery.Read.All、eDiscovery.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/legalHolds
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) 对象的 JSON 表示形式。

创建 **ediscoveryHoldPolicy** 时，可以指定以下属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|法定保留策略的显示名称。 必需。|
|description|String|法律保留策略的说明。 可选。|
|contentQuery|String|法定保留策略的内容查询。 可选。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_ediscoveryholdpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/legalHolds
Content-Type: application/json

{
    "displayname": "My legalHold with sources",
    "description": "Created from Graph API",
    "contentQuery": "Bazooka",
    "userSources@odata.bind": [
        {
            "@odata.type": "microsoft.graph.security.userSource",
            "email": "SalesTeam@M365x809305.OnMicrosoft.com"
        }
    ],
    "siteSources@odata.bind": [
        {
            "@odata.type": "microsoft.graph.security.siteSource",
            "site": {
                "webUrl": "https://m365x809305.sharepoint.com/sites/Design-topsecret"
            }
        }
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-ediscoveryholdpolicy-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-ediscoveryholdpolicy-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-ediscoveryholdpolicy-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-ediscoveryholdpolicy-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-ediscoveryholdpolicy-from--powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>响应
下面是响应的示例
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryHoldPolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/legalHolds/$entity",
    "isEnabled": true,
    "errors": [],
    "contentQuery": "Bazooka",
    "description": "Created from Graph API",
    "createdDateTime": "2022-05-23T03:54:11.1Z",
    "lastModifiedDateTime": "2022-05-23T03:54:11.1Z",
    "status": "pending",
    "id": "b9758bbc-ddbd-45e0-8484-3eb49cf1ded3",
    "displayName": "My legalHold with sources",
    "createdBy": {
        "application": null,
        "user": {
            "id": "MOD Administrator",
            "displayName": null
        }
    },
    "lastModifiedBy": {
        "application": null,
        "user": {
            "id": "MOD Administrator",
            "displayName": null
        }
    }
}
```

