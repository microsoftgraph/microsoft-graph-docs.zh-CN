---
title: 创建 noncustodialDataSource
description: 创建新的 noncustodialDataSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 87817dfed8b4ba12c98661e847aa7e44302a7771
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080735"
---
# <a name="create-noncustodialdatasource"></a>创建 noncustodialDataSource

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) 对象。

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
POST /compliance/ediscovery/cases/{caseId}/noncustodialDataSources
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
|applyHoldToSource|Boolean|指示是否将保留应用于非 (数据源，如邮箱或网站) 。|
|datasource|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|userSource 或 siteSource。  对于 userSource，请使用"dataSource" ： { "@odata.type" ： "microsoft.graph.ediscovery.userSource"， "email" ： "SMTP address"}。  对于网站源，请使用"dataSource" ： { "@odata.type" ： "microsoft.graph.ediscovery.siteSource"， "site@odata.bind" ： "siteId" }，其中 siteId 可以派生自网站 URL，例如，Microsoft Graph 请求为 `https://contoso.sharepoint.com/sites/HumanResources` `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` 。 ID 是 ID 字段中列出的第一个 GUID。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和非 `201 Created` [custodialDataSource](../resources/ediscovery-noncustodialdatasource.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_noncustodialdatasource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources
Content-Type: application/json
Content-length: 206

{
    "applyHoldToSource" : true,
    "dataSource" : {
        "@odata.type" : "microsoft.graph.ediscovery.userSource",
        "email" : "adelev@contoso.com"
    }
}
```

### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/noncustodialDataSources/$entity",
    "status": "0",
    "lastModifiedDateTime": "2021-02-19T07:02:45.7732516Z",
    "releasedDateTime": "0001-01-01T00:00:00Z",
    "id": "39374346363831303741353341373443",
    "displayName": null,
    "createdDateTime": "2021-02-19T07:02:45.4863718Z",
    "applyHoldToSource": true
}
```
