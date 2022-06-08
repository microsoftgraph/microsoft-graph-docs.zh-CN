---
title: 列出 additionalSources
description: 从 additionalSources 导航属性获取 ediscoveryNoncustodialDataSource 资源。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 3434d6e084baccace66d24f25d7beb5eb76a65c9
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945429"
---
# <a name="list-additionalsources"></a>列出 additionalSources
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从 additionalSources 导航属性获取 ediscovery 数据源资源。

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
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/additionalSources
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

如果成功，此方法返回 `200 OK` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "list_ediscoverynoncustodialdatasource"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches/c61a5860-d634-4d14-aea7-d82b6f4eb7af/additionalSources
```


### <a name="response"></a>响应
下面是响应的示例
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.ediscoveryNoncustodialDataSource)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/searches('c61a5860-d634-4d14-aea7-d82b6f4eb7af')/additionalSources",
    "value": [
        {
            "@odata.type": "#microsoft.graph.security.userSource",
            "displayName": null,
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "43434642-3137-3138-3432-374142313639",
            "email": "AlexW@M365x809305.OnMicrosoft.com",
            "includedSources": "mailbox",
            "siteWebUrl": null,
            "createdBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.userSource",
            "displayName": null,
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "38423145-4639-4244-4437-464630424139",
            "email": "IrvinS@M365x809305.OnMicrosoft.com",
            "includedSources": "mailbox",
            "siteWebUrl": null,
            "createdBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.userSource",
            "displayName": null,
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "36304536-3033-3845-4639-394538443235",
            "email": "AllanD@M365x809305.OnMicrosoft.com",
            "includedSources": "mailbox",
            "siteWebUrl": null,
            "createdBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.siteSource",
            "@odata.id": "https://graph.microsoft.com/v1.0/sites/",
            "displayName": null,
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "46454445-3936-3941-4145-463642313642",
            "createdBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.siteSource",
            "@odata.id": "https://graph.microsoft.com/v1.0/sites/",
            "displayName": null,
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "37383041-3143-3731-3744-384643453341",
            "createdBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.siteSource",
            "@odata.id": "https://graph.microsoft.com/v1.0/sites/",
            "displayName": null,
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "30394337-4541-4632-4532-423832464235",
            "createdBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        }
    ]
}
```

