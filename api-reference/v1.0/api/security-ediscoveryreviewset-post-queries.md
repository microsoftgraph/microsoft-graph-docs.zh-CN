---
title: 创建 ediscoveryReviewSetQuery
description: 创建新的 ediscoveryReviewSetQuery 对象。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 160bb50fe1e4a2f00b75f90d7047fc49e9bb0492
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839137"
---
# <a name="create-ediscoveryreviewsetquery"></a>创建 ediscoveryReviewSetQuery
命名空间：microsoft.graph.security



创建新的 [ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) 对象。

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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/queries
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) 对象的 JSON 表示形式。

创建 **ediscoveryReviewSetQuery** 时，可以指定以下属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|查询的名称。 必需。|
|contentQuery|String|审阅集的 KQL 查询。 有关详细信息，请参阅 [审阅集中的查询和筛选内容](/microsoft-365/compliance/review-set-search)。|



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "create_ediscoveryreviewsetquery_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/queries
Content-Type: application/json

{
    "displayName": "My Query 1",
    "contentQuery": "(Author=\"edison\")"
}
```


### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryReviewSetQuery"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#security/cases/ediscoveryCases('58399dff-cebe-478f-b1af-d3227f1fd645')/reviewSets('273f11a1-17aa-419c-981d-ff10d33e420f')/queries/$entity",
    "description": null,
    "lastModifiedDateTime": "2022-05-29T23:39:51.3307953Z",
    "contentQuery": "((Author=\"edison\"))",
    "id": "fcb86cd1-50e0-427c-840e-ba6f087364e5",
    "displayName": "My Query 1",
    "createdDateTime": "2022-05-29T23:39:51.3307953Z",
    "createdBy": {
        "application": null,
        "user": {
            "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
            "displayName": null,
            "userPrincipalName": "c25c3914-f9f7-43ee-9cba-a25377e0cec6"
        }
    },
    "lastModifiedBy": {
        "application": null,
        "user": {
            "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
            "displayName": null,
            "userPrincipalName": "c25c3914-f9f7-43ee-9cba-a25377e0cec6"
        }
    }
}
```

