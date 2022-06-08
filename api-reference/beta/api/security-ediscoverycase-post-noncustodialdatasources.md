---
title: 创建 ediscoveryNoncustodialDataSource
description: 创建新的 ediscoveryNoncustodialDataSource 对象。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 77c763fa5e14e795055976ef74fb315c10a96cb7
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945517"
---
# <a name="create-ediscoverynoncustodialdatasource"></a>创建 ediscoveryNoncustodialDataSource
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 ediscoveryNoncustodialDataSource 对象。

## <a name="permissions"></a>权限
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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/noncustodialDataSources
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) 对象的 JSON 表示形式。

创建 **ediscoveryNoncustodialDataSource** 时，可以指定以下属性。

|属性|类型|说明|
|:---|:---|:---|
|dataSource|[microsoft.graph.security.dataSource](../resources/security-datasource.md)|必填。 userSource 或 siteSource。 对于 userSource，请使用“dataSource”： { “@odata.type”： “microsoft.graph.security.userSource”， “email” ： “SMTP address”}。  对于站点源，请使用“dataSource”： { “@odata.type”： “microsoft.graph.security.siteSource”， “site@odata.bind” ： “siteId” }， where siteId can deriv from the site URL， 例如 `https://contoso.sharepoint.com/sites/HumanResources`， Microsoft Graph request be `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources`. ID 是 ID 字段中列出的第一个 GUID。 或者直接使用 webUrl，“dataSource”： {“@odata.type”： “microsoft.graph.security.siteSource”，“site”： {“webUrl”： `https://m365x809305.sharepoint.com/sites/Design-topsecret`}}



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "create_ediscoverynoncustodialdatasource_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialDataSources
Content-Type: application/json

{
    "dataSource": {
        "@odata.type": "microsoft.graph.security.siteSource",
        "site": {
            "webUrl": "https://m365x809305.sharepoint.com/sites/Design-topsecret"
        }
    }
}
```


### <a name="response"></a>响应
下面是响应的示例
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryNoncustodialDataSource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/noncustodialDataSources/$entity",
    "status": "active",
    "holdStatus": "notApplied",
    "createdDateTime": "2022-05-23T03:15:08.5354451Z",
    "lastModifiedDateTime": "2022-05-23T03:15:08.5354451Z",
    "releasedDateTime": "0001-01-01T00:00:00Z",
    "id": "43373338343345303943344434423032",
    "displayName": "Design - top secret"
}
```
