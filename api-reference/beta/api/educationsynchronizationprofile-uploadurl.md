---
title: 'educationSynchronizationProfile: uploadUrl'
description: 将源文件上载到租户中的特定学校数据同步配置文件的 Azure blob 存储检索共享的访问签名 (SA)。 SAS 令牌具有一小时的有效性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 74f37f5653147691c408cf83e3039920957352c7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511595"
---
# <a name="educationsynchronizationprofile-uploadurl"></a>educationSynchronizationProfile: uploadUrl

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将源文件上载到租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的 Azure blob 存储检索共享的访问签名 (SA)。 SAS 令牌具有一小时的有效性。

上载[CSV 数据提供](../resources/educationcsvdataprovider.md)程序仅提供 URL。

> **注意：** 若要访问与 SAS 令牌对 blob 存储，请使用[Azure 存储 Sdk](https://github.com/search?q=org%3AAzure+azure-storage)或[AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限 |
|:-----------|:----------|
| 委派（工作或学校帐户） | EduAdministration.ReadWrite |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
## <a name="response"></a>响应
如果成功，此方法返回`200 OK`响应代码和响应正文中[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) SAS URL。

如果仍在处理的上一个请求，此方法返回`409 Conflict`，指出上载的[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)目前被阻止。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```

##### <a name="response"></a>响应
下面展示了示例响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "@odata.type": "String",
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 314

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#String",
    "value": "https://sdsstorage.blob.core.windows.net/86904b1e-c7d0-4ead-b13a-98f11fc400ee?sv=2015-07-08&sr=c&si=SharedAccessPolicy_20170704044441&sig=CH65vxxqXETCkQNH0Lfsu31cUo0s0XcEEo0OE2YiL6Q%3D&se=2017-07-04T08%3A43%3A01Z&sp=w"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-uploadurl.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
