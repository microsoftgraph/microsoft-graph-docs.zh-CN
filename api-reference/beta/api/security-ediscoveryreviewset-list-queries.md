---
title: 列出 ediscoveryReviewSetQuery
description: 从 reviewSetQuery 导航属性获取 ediscoveryReviewSetQuery 资源。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 5aed7e46ba4655111485a14b3671766f869c93cc
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945447"
---
# <a name="list-ediscoveryreviewsetquery"></a>列出 ediscoveryReviewSetQuery
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从 reviewSetQuery 导航属性获取 ediscoveryReviewSetQuery 资源。

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
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/queries
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

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) 对象的集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "list_ediscoveryreviewsetquery"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/queries
```


### <a name="response"></a>响应
下面是响应的示例
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.ediscoveryReviewSetQuery)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('58399dff-cebe-478f-b1af-d3227f1fd645')/reviewSets('273f11a1-17aa-419c-981d-ff10d33e420f')/queries",
    "value": [
        {
            "lastModifiedDateTime": "2022-05-29T20:49:47.9289317Z",
            "contentQuery": "((((FileClass=\"Email\") AND (InclusiveType=\"InclusiveMinus\" OR InclusiveType=\"Inclusive\")) OR ((FileClass=\"Attachment\") AND (UniqueInEmailSet=\"true\")) OR ((FileClass=\"Document\") AND (MarkAsRepresentative=\"Unique\")) OR ((FileClass=\"Conversation\"))))",
            "id": "837335b0-1943-444d-a3d1-5522cc21c5a4",
            "displayName": "[AutoGen] For Review",
            "createdDateTime": "2022-05-29T20:49:47.9289317Z",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            },
            "lastModifiedBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            }
        },
        {
            "lastModifiedDateTime": "2022-05-29T20:49:48.0539099Z",
            "contentQuery": "((FileType:gz OR FileType:gzip OR FileType:bz2 OR FileType:zip OR FileType:7z OR FileType:rar OR FileType:vhd OR FileType:mbox OR FileType:pst OR FileType:sfx) OR (Size<\"3072B\" AND (FileType:gif OR FileType:bmp OR FileType:png OR FileType:jpg OR FileType:jpeg OR FileType:tif OR FileType:tiff OR FileType:emf OR FileType:pct OR FileType:pic)))",
            "id": "977ad4d5-3e5c-4594-8cb6-7d09dbcddf21",
            "displayName": "[AutoGen] Potentially Immaterial Items",
            "createdDateTime": "2022-05-29T20:49:48.0539099Z",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            },
            "lastModifiedBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            }
        }
    ]
}
```

