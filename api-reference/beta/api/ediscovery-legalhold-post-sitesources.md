---
title: 创建 legalHold siteSource
description: 创建新的 legalHold siteSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: dd6710bd04c392c144080dc64ba9c962f99c567a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446039"
---
# <a name="create-legalhold-sitesource"></a>创建 legalHold siteSource

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将 siteSource 添加到 legalHold 对象。

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
POST /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/siteSources
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [siteSource](../resources/ediscovery-sitesource.md) 对象的 JSON 表示形式。

下表显示创建 [siteSource](../resources/ediscovery-sitesource.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|site@odata.bind|String|网站的 ID，您可以通过使用路径方法获取网站[资源从网站资源获取 ID。](../api/site-getbypath.md) [](../resources/site.md) 用法为 {hostname}：/{relative-path}。 对于网站 `https://contoso.sharepoint.com/sites/HumanResources` URL，Microsoft Graph 请求为 `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` 。 ID 是 ID 字段中列出的第一个 GUID。  对于 OneDrive for Business 网站 `https://contoso-my.sharepoint.com/personal/adelev_contoso_com` URL，Microsoft Graph 请求为 `https://graph.microsoft.com/v1.0/sites/contoso-my.sharepoint.com:/personal/adelev_contoso_com` |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码和 `201 Created` [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_sitesource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/387566cc-38ae-4e85-ab4b-cd2dd34faa07/siteSources
Content-Type: application/json
Content-length: 154

{
    "site@odata.bind": "https://graph.microsoft.com/v1.0/sites/50073f3e-cb22-48e5-95a9-51a3da455181"
}
```

### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.siteSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('c816dd6f-5af8-40c5-a760-331361e05c60')/legalHolds('387566cc-38ae-4e85-ab4b-cd2dd34faa07')/siteSources/$entity",
    "displayName": "Adele Vance",
    "createdDateTime": "2020-12-28T20:08:57.857Z",
    "id": "50073f3e-cb22-48e5-95a9-51a3da455181",
    "createdBy": {
        "user": {
            "id": null,
            "displayName": "EDiscovery admin"
        }
    }
}
```
