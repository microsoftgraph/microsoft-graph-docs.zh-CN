---
title: 获取 sourceCollection
description: 读取 sourceCollection 对象的属性和关系。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: b10f29de6bbf61151f55aae2a37ac10ddf3ece86
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446005"
---
# <a name="get-sourcecollection"></a>获取 sourceCollection

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [sourceCollection 对象的属性和](../resources/ediscovery-sourcecollection.md) 关系。

## <a name="permissions"></a>Permissions

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
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

用于 `$expand` 展开审阅集操作、保管人源和上次估计统计信息操作。

```http
https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourcecollections/1a9b4145d8f84e39bc45a7f68c5c5119?$expand=addToReviewSetOperation,custodianSources,lastEstimateStatisticsOperation
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码和 `200 OK` [microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get_sourcecollection"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourcecollections/1a9b4145d8f84e39bc45a7f68c5c5119?$expand=addToReviewSetOperation,custodianSources,lastEstimateStatisticsOperation
```

### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.sourceCollection"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('47746044-fd0b-4a30-acfc-5272b691ba5b')/sourceCollections/$entity",
    "description": null,
    "lastModifiedDateTime": "2021-01-12T18:09:03.7378679Z",
    "contentQuery": "subject:'Quarterly Financials'",
    "tenantSources": "none",
    "id": "1a9b4145d8f84e39bc45a7f68c5c5119",
    "displayName": "Quarterly Financials search",
    "createdDateTime": "2021-01-12T18:09:03.417009Z",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalname": "admin@contoso.com"
        }
    },
    "lastModifiedBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalname": "admin@contoso.onmicrosoft.com"
        }
    },
    "addToReviewSetOperation": {
        "createdDateTime": "2021-01-13T05:38:49.9186654Z",
        "completedDateTime": "2021-01-13T07:54:45.0007868Z",
        "percentProgress": 100,
        "status": "succeeded",
        "action": "addToReviewSet",
        "id": "aef586b34d89405d802497658a14194f",
        "createdBy": {
            "user": {
                "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                "displayName": null,
                "userPrincipalName": "admin@contoso.com"
            }
        }
    },
    "lastEstimateStatisticsOperation": {
        "createdDateTime": "2021-01-12T21:53:50.7272654Z",
        "completedDateTime": "2021-01-12T21:54:49.5595543Z",
        "percentProgress": 100,
        "status": "succeeded",
        "action": "estimateStatistics",
        "id": "f3db0382af0842eaa98c7dd59e7dace6",
        "indexedItemCount": 39598,
        "indexedItemsSize": 3760920737,
        "unindexedItemCount": 0,
        "unindexedItemsSize": 0,
        "mailboxCount": 1,
        "siteCount": 1,
        "createdBy": {
            "user": {
                "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                "displayName": "EDisco Admin",
                "userPrincipalName": "admin@contoso.com"
            }
        }
    }
}
```
