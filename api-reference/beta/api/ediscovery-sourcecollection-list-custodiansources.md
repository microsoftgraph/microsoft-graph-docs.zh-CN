---
title: 列出 custodianSources
description: 获取与源集合关联的 DataSource 对象列表。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: eea1456727089f90a2045ba3ca9d54c12fa792ac
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446000"
---
# <a name="list-custodiansources"></a>列出 custodianSources

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取与 [源集合关联的 DataSource](../resources/ediscovery-datasource.md) 对象列表。

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
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/custodianSources
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

如果成功，此方法在响应正文中返回响应代码和 `200 OK` [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "list_datasource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/custodianSources
```

### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.dataSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ediscovery.dataSource",
      "id": "0fb67fc5-7fc5-0fb6-c57f-b60fc57fb60f",
      "displayName": "String",
      "createdDateTime": "String (timestamp)",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      }
    }
  ]
}
```
