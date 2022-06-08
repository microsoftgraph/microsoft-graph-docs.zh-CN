---
title: 列出 ediscoveryEstimateOperations
description: 获取最后一个 ediscoveryEstimateOperation 对象及其属性。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 6b60faca5c61b9c5ebaf1fb87c42a2a117104f33
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945434"
---
# <a name="list-ediscoveryestimateoperations"></a>列出 ediscoveryEstimateOperations
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取最后  [一个 ediscoveryEstimateOperation](../resources/security-ediscoveryestimateoperation.md) 对象及其属性。

>**注意：** 此方法仅列出最后一个操作;它不会返回所有操作的历史记录。

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
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/lastEstimateStatisticsOperation
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

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ediscoveryEstimateOperation](../resources/security-ediscoveryestimateoperation.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "list_ediscoveryestimateoperation"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches/c61a5860-d634-4d14-aea7-d82b6f4eb7af/lastEstimateStatisticsOperation
```


### <a name="response"></a>响应
下面是响应的示例
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryEstimateOperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.security.ediscoveryEstimateOperation",
    "createdDateTime": "2022-05-29T18:56:48.4649404Z",
    "completedDateTime": "2022-05-29T18:58:31.968065Z",
    "percentProgress": 100,
    "status": "succeeded",
    "action": "estimateStatistics",
    "id": "d80d2f2bc71d4544b75d4836bef4ff57",
    "indexedItemCount": 1756,
    "indexedItemsSize": 89489297,
    "unindexedItemCount": 1,
    "unindexedItemsSize": 57952,
    "mailboxCount": 4,
    "siteCount": 6,
    "createdBy": {
        "application": null,
        "user": {
            "id": "0d38933a-0bbd-41ca-9ebd-28c4b5ba7cb7",
            "displayName": null,
            "userPrincipalName": null
        }
    }
}
```

