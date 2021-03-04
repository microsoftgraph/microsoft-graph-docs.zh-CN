---
title: sourceCollection：estimateStatistics
description: 运行源集合的估计值。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 7489f2900ef79afc95cdc00c47569a63b378572f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446010"
---
# <a name="sourcecollection-estimatestatistics"></a>sourceCollection：estimateStatistics

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

运行源集合中电子邮件和文档的估计数量。 若要了解有关电子数据展示 (搜索的源集合) ，请参阅"在高级电子数据展示"中收集 [案例的数据](https://docs.microsoft.com/microsoft-365/compliance/collecting-data-for-ediscovery)。

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
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/estimateStatistics
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果估计成功启动，此操作将返回 `202 Accepted` 响应代码。 响应还将包含一个标头，其中包含为处理估计而创建的 `Location` [estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md) 的位置。 通过向位置提出 GET 请求来检查估计操作的状态，成功完成后， [状态将更改为](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) `succeeded` 。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "sourcecollection_estimatestatistics"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/estimateStatistics
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
cache-control: private
client-request-id: af32de50-99d9-e3a8-371b-a4f366cc78e7
content-length: 0
content-type: text/plain
location: https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/operations/82edd40e182a464fa02c24a36fa94873
request-id: e890176f-640f-4222-9cd8-be26e71c5e5d
```
