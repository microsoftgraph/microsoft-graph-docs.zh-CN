---
title: reviewSetQuery：applyTags
description: 将标记应用于与指定查询匹配的文档。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2c3f41d1fbe9851babc582c1f21c9f9673d53541
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446025"
---
# <a name="reviewsetquery-applytags"></a>reviewSetQuery：applyTags

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
POST /compliance/ediscovery/cases/{caseId}/reviewSets/{reviewSetId}/queries/{reviewSetQueryId}/applyTags
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|说明|
|:---|:---|:---|
|tagsToAdd|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 集合|要添加到与查询匹配的文档的标记的标识。|
|tagsToRemove|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 集合|要从匹配查询的文档中删除的标记的标识。|

## <a name="response"></a>响应

如果成功，此操作返回 `202 Accepted` 响应代码。

如果标记操作成功启动，此操作将返回 `202 Accepted` 响应代码。 响应还将包含一个标头，其中包含为处理标记而创建的 `Location` [tagOperation](../resources/ediscovery-tagOperation.md) 的位置。 通过向位置提出 GET 请求来检查标记操作的状态，成功完成后， [状态将更改为](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) `succeeded` 。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "reviewsetquery_applytags"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/reviewsets/6c95c2a6-31fa-45a8-93ef-dd4531974783/queries/b4798d14-748d-468e-a1ec-96a2b1d49677/applyTags
Content-Type: application/json
Content-length: 778

{
    "tagsToAdd": [
        {
            "id": "b4798d14-748d-468e-a1ec-96a2b1d49677"
        }
    ]
}
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
cache-control: no-cache,
client-request-id: 56c9dd8b-d8f7-59ae-6733-38191862c9c9,
location: https://graph.microsoft.com/beta/compliance/ediscovery/cases('47746044-fd0b-4a30-acfc-5272b691ba5b')/operations('d77f7933e88842bab3221e280be9dc0b'),
request-id: c2397a81-e9c2-4851-b669-d87e0751e45a
```
