---
title: 删除标记
description: 删除标记对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 1ec395a45ee3720797228952b1f9047822fed11c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445985"
---
# <a name="delete-tag"></a>删除标记

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除 [标记](../resources/ediscovery-tag.md) 对象。

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
DELETE /compliance/ediscovery/cases/{caseId}/tags/{tagId}?forcedelete=true
```

## <a name="query-parameters"></a>查询参数

在请求 URL 中，提供以下所需的查询参数。

| 参数     | 类型    | 说明                                                                              |
|:--------------|:--------|:-----------------------------------------------------------------------------------------|
| forcedelete   | 布尔 | 如果设置为 true，则删除标记和子项（如果为 false）并且标记具有子项，则删除将失败。 |

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "delete_tag"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/9985bd266f2f459cbebc81522734b452?forcedelete=true
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
