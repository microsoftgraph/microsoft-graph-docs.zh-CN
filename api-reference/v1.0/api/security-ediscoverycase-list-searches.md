---
title: 列出搜索
description: 从电子数据展示案例中获取搜索列表
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 0ebd054f1efd698ed387314b258f64127d4a08ce
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839204"
---
# <a name="list-searches"></a>列出搜索
命名空间：microsoft.graph.security



从 [eDiscoveryCase](../resources/security-ediscoverycase.md) 对象获取 [ediscoverySearch](../resources/security-ediscoverysearch.md) 资源的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|eDiscovery.Read.All、eDiscovery.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches
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

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md) 对象的集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "list_ediscoverysearch"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches
```


### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.ediscoverySearch)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/searches",
    "value": [
        {
            "dataSourceScopes": "none",
            "description": "My first search",
            "lastModifiedDateTime": "2022-05-23T04:38:07.5787454Z",
            "contentQuery": "(Author=\"edison\")",
            "id": "46867792-68e6-41db-9cd0-f651c2290d91",
            "displayName": "My search 2",
            "createdDateTime": "2022-05-23T04:38:07.5787454Z",
            "lastModifiedBy": null,
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                },
                "application": {
                    "id": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
                    "displayName": "Graph Explorer"
                }
            }
        },
        {
            "dataSourceScopes": "none",
            "description": "My first search",
            "lastModifiedDateTime": "2022-05-23T04:35:36.5424818Z",
            "contentQuery": "(Author=\"edison\")",
            "id": "80b9d59a-12a6-4273-a3d4-ab78f9a04ea5",
            "displayName": "My search 1",
            "createdDateTime": "2022-05-23T04:35:36.5424818Z",
            "lastModifiedBy": null,
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                },
                "application": {
                    "id": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
                    "displayName": "Graph Explorer"
                }
            }
        }
    ]
}
```

