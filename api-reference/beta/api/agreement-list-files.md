---
title: '列出 (本地化协议文件) '
description: 检索与协议相关的所有本地化文件。
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 9679e1e26867130c5ae44cbc2bf0b3fafc6aa110
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516197"
---
# <a name="list-files-localized-agreement-files"></a>列出 (本地化协议文件) 
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索与协议相关的所有本地化文件。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | Agreement.Read.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|Application                            | 不支持。 |


## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /agreements/{agreementsId}?$expand=files
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [agreementFileLocalization](../resources/agreementfilelocalization.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_agreementfilelocalization"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/94410bbf-3d3e-4683-8149-f034e55c39dd?$expand=files
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-agreementfilelocalization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-agreementfilelocalization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-agreementfilelocalization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-agreementfilelocalization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-agreementfilelocalization-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-agreementfilelocalization-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementFileLocalization"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#agreements(files())/$entity",
    "id": "94410bbf-3d3e-4683-8149-f034e55c39dd",
    "displayName": "Contoso ToU for guest users",
    "termsExpiration": null,
    "userReacceptRequiredFrequency": null,
    "isViewingBeforeAcceptanceRequired": true,
    "isPerDeviceAcceptanceRequired": false,
    "files@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/termsOfUse/agreements('94410bbf-3d3e-4683-8149-f034e55c39dd')/files",
    "files": [
        {
            "id": "08033369-8972-42a3-8533-90bbd2757a01",
            "fileName": "TOU.pdf",
            "displayName": "Contoso ToU for guest users",
            "language": "en",
            "isDefault": true,
            "isMajorVersion": false,
            "createdDateTime": "2022-03-04T13:14:13.9361722Z",
            "fileData": null
        },
        {
            "id": "90d1723c-52c1-40e3-a51a-da99a82c0327",
            "fileName": "Contoso ToU for guest users (French)",
            "displayName": "Contoso ToU for guest users (French)",
            "language": "fr-FR",
            "isDefault": false,
            "isMajorVersion": false,
            "createdDateTime": "2022-03-04T14:38:22.8292386Z",
            "fileData": null
        }
    ]
}
```

