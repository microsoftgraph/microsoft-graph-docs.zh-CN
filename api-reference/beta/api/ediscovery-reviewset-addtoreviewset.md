---
title: reviewSet：addToReviewSet
description: 开始将 Microsoft 365 服务中的集合添加到审阅集的过程。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 4eb0a7c2de533332c57f3e26d3b6fba25a68259d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720373"
---
# <a name="reviewset-addtoreviewset"></a>reviewSet：addToReviewSet

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

开始将 Microsoft 365 服务中的集合添加到审阅集的过程。 创建操作后，可以通过从响应标头中检索参数获取 `Location` 操作的状态。 该位置提供将返回 [caseExportOperation 的](../resources/ediscovery-caseexportoperation.md)URL。

## <a name="permissions"></a>Permissions

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
POST /compliance/ediscovery/cases/{caseId}/reviewSets/{reviewsetId}/addToReviewSet
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
|sourceCollection|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|**sourceCollection 的** ID。|
|additionalData|[microsoft.graph.ediscovery.dataCollectionScope](../resources/ediscovery-addtoreviewsetoperation.md#datacollectionscope-values)|**集合中将包含的 dataCollectionScope。**|

## <a name="response"></a>响应

如果成功，此操作返回 `202 Accepted` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "reviewset_addtoreviewset"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/080e8cad-f21f-4452-8826-0ddf7e949fdd/reviewSets/6fe25d32-8167-4625-b75c-c4181ccbd9d5/addToReviewSet
Content-Type: application/json
Content-length: 531

{
    "sourceCollection": {
        "id": "1a9b4145d8f84e39bc45a7f68c5c5119"
    },
    "additionalData": "linkedFiles"
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
```
