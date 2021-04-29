---
title: 添加 noncustodialDataSource
description: 通过发布到 noncustodialSources 集合添加 noncustodialSources。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 399d20f5bc046d141e8652001fe964460c2b414c
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080733"
---
# <a name="add-noncustodialdatasource"></a>添加 noncustodialDataSource

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将 noncustodialSources 添加到 [sourceCollection](../api/ediscovery-sourcecollection-get.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|eDiscovery.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/noncustodialSources/$ref
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) 对象的 JSON 表示形式。

下表显示创建 [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|@odata.id|String|定义空心对象的字符串。 请参阅下面的示例。  @odata.id 可以从 [非custodialDataSource 中检索](../resources/ediscovery-noncustodialdatasource.md)。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和非 `204 No Content` [custodialDataSource](../resources/ediscovery-noncustodialdatasource.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_noncustodialdatasource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/sourceCollections/12aab1671c834213a84ba219c06f4c5a/noncustodialSources/$ref
Content-Type: application/json
Content-length: 206

{
    "@odata.id": "https://canary.graph.microsoft.com/testprodbetancsdsaslist/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/noncustodialDataSources/39383530323537383742433232433246"
}
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource"
}
-->

``` http
HTTP/1.1 204 No Content
```
