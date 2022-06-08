---
title: 列出保管人来源
description: 从 CustodianSources 导航属性获取 dataSource 资源。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: c28295043399f72181a134915e7edf42584331eb
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945481"
---
# <a name="list-custodiansources"></a>列出保管人来源
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从 CustodianSources 导航属性获取 dataSource 资源。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|eDiscovery.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/custodianSources
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

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [dataSource](../resources/security-datasource.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "list_datasource"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches/c61a5860-d634-4d14-aea7-d82b6f4eb7af/custodianSources
```


### <a name="response"></a>响应
下面是响应的示例
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.dataSource)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.security.dataSource)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.security.userSource",
            "@odata.id": "https://graph.microsoft.com/beta/security/cases/cases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/userSources('c25c3914-f9f7-43ee-9cba-a25377e0cec6')",
            "displayName": "MOD Administrator",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
            "email": "admin@M365x809305.onmicrosoft.com",
            "includedSources": "mailbox,site",
            "siteWebUrl": null,
            "createdBy": {
                "application": null,
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.userSource",
            "@odata.id": "https://graph.microsoft.com/beta/security/cases/cases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/userSources('43434642-3137-3138-3432-374142313639')",
            "displayName": "Alex Wilber",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "43434642-3137-3138-3432-374142313639",
            "email": "AlexW@M365x809305.OnMicrosoft.com",
            "includedSources": "mailbox,site",
            "siteWebUrl": null,
            "createdBy": {
                "application": null,
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.unifiedGroupSource",
            "@odata.id": "https://graph.microsoft.com/beta/security/cases/cases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/unifiedGroupSources('32e14fa4-3106-4bd2-a245-34bf0c718a7e')",
            "displayName": "Design (Mailbox)",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "32e14fa4-3106-4bd2-a245-34bf0c718a7e",
            "includedSources": "mailbox,site",
            "createdBy": {
                "application": null,
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.siteSource",
            "@odata.id": "https://graph.microsoft.com/beta/security/cases/cases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/siteSources('169718e3-a8df-449d-bef4-ee09fe1ddc5d')",
            "displayName": "U.S. Sales",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "169718e3-a8df-449d-bef4-ee09fe1ddc5d",
            "createdBy": {
                "application": null,
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.userSource",
            "@odata.id": "https://graph.microsoft.com/beta/security/cases/cases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('c25c3914f9f743ee9cbaa25377e0cec6')/userSources('45354430-3730-4232-4236-323230383438')",
            "displayName": "MOD Administrator",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "45354430-3730-4232-4236-323230383438",
            "email": "admin@M365x809305.onmicrosoft.com",
            "includedSources": "mailbox,site",
            "siteWebUrl": null,
            "createdBy": {
                "application": null,
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": null
                }
            }
        }
    ]
}
```

